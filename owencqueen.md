# Open Source Assignments

## Sprint 1
I have been assigned [Instance 752](https://davidalanreid.github.io/output/347538efbdc21b8df684ebd92d37400b3ce85d55/vulnerable.hack.html) and [Instance 300](https://davidalanreid.github.io/output/347538efbdc21b8df684ebd92d37400b3ce85d55/vulnerable.hack.html). I have used the following criteria to determine if the projects are still active:
1. Recency of updates
2. Number of contributors
3. Frequency of updates
4. Pull requests and issues open

### Instance 752
This instance is from a repository named "One Thousand Years", and its a utility engine for game development. It has several contributors to the project as well as multiple branches where people have made contributions. However, the last
commit for this file was on May 25, 2020, about 10 months ago. While the project was active before then (lots of commits, merges, etc.), there has been little-to-no activity since that last commit, including no issues or pull requests. Because of this, I have determined
that this project is inactive.

### Instance 300
This instance is from a library named "DEngine-pcsv4", which is a low-level 3d graphics library written primarily in C++. This project is managed mainly by the repository owner, so all contributions must be made through pull request.
This project has distinct "releases", meaning that they release groups of edits to the code all at one time. The last of these releases was committed on Dec. 25, 2020, so within the last 3 months. However, there are no listed issues or pull requests. If this repo accepted incremental pull
requests, this would normally indicate that the project is stagnant, but since there are distinct releases, this could indicate an active project. There have been 3 major releases in past year, so by this criteria, I determine that this
project is indeed active.

## Sprint 2
I will now determine if either of my assigned project are accepting contributions. I have used the following criteria to determine this:
1. Recency of accepted pull requests
2. Frequency of pull requests
3. Responses of contributors to issues
4. Instructions included in README about how to contribute

### Instance 752
As previously stated, this project is not active, so they are also not accepting contributions. This can be seen by the fact that there are no open pull requests, and nothing has been committed to the repo at all in the last 10 months. There are also no open or closed issues, meaning that the contributors have not been actively responding to user input on the problems in the repo.

### Instance 300
This project appears to be accepting contributions. While there are no active pull requests, the repo manager has also turned off a lot of visibility to the repo, including issues, so if there were open issues/pull requests, I would have no idea. Since this project is active though, and they list instructions to contribute in the README, I would say that they are open to receiving contributions and just haven't seen any submissions lately. 

## Sprint 3
For this sprint, we have been assigned to determine if our assigned vulnerability still exists in each of the instances.

### Instance 752
The vulnerability that I was assigned still exists in two files, but it seems to have been resolved in the other files that would normally have the vulnerability. The contributors to the repository seem to have added additional functionality to accomplish the goals sought by `libpng`'s fix to the vulnerability, so I would say the vulnerability has been resolved for two of the files. To determine this, I ran `diff` on the files from the commit that fixed the vulnerability in `libpng` and the corresponding files in `global-engine`. 

### Instance 300
The vulnerability for this issue still exits in the main `DEngine-pcsx4` repository. To determine this, I cloned the `DEngine-pcsx4` as well as the `libpng` repository and ran `diff` between the files that were changed on the given commit in `libpng`. After running `diff`, I saw that the issue fixed by the more recent update of `libpng` was still present in `DEngine-pcsx4`.

## Sprint 4

### Instance 752
Here is the patch from my contribution:
```
diff --git a/deps/cegui-dependencies/src/FreeImage-3.15.0/Source/LibPNG/pngrutil.c b/deps/cegui-dependencies/src/FreeImage-3.15.0/Source/LibPNG/pngrutil.c
index 5429887a..24434e2c 100644
--- a/deps/cegui-dependencies/src/FreeImage-3.15.0/Source/LibPNG/pngrutil.c
+++ b/deps/cegui-dependencies/src/FreeImage-3.15.0/Source/LibPNG/pngrutil.c
@@ -144,6 +144,23 @@ png_read_chunk_header(png_structp png_ptr)
    png_reset_crc(png_ptr);
    png_calculate_crc(png_ptr, png_ptr->chunk_name, 4);

+   //Addition: owencqueen, 03/28/2021
+   /* Check for too-large chunk length */
+   if (png_ptr->chunk_name != png_IDAT)
+   {
+      png_alloc_size_t limit = PNG_SIZE_MAX;
+# ifdef PNG_SET_USER_LIMITS_SUPPORTED
+      if (png_ptr->user_chunk_malloc_max > 0 &&
+          png_ptr->user_chunk_malloc_max < limit)
+         limit = png_ptr->user_chunk_malloc_max;
+# elif PNG_USER_CHUNK_MALLOC_MAX > 0
+      if (PNG_USER_CHUNK_MALLOC_MAX < limit)
+         limit = PNG_USER_CHUNK_MALLOC_MAX;
+# endif  
+      if (length > limit)
+         png_chunk_error(png_ptr, "chunk data is too large");
+   }     
+
    /* Check to see if chunk name is valid. */
    png_check_chunk_name(png_ptr, png_ptr->chunk_name);

diff --git a/deps/cegui-dependencies/src/libpng-1.4.7/pngrutil.c b/deps/cegui-dependencies/src/libpng-1.4.7/pngrutil.c
index 113589c6..29f3b11b 100644
--- a/deps/cegui-dependencies/src/libpng-1.4.7/pngrutil.c
+++ b/deps/cegui-dependencies/src/libpng-1.4.7/pngrutil.c
@@ -147,6 +147,23 @@ png_read_chunk_header(png_structp png_ptr)
    /* Check to see if chunk name is valid. */
    png_check_chunk_name(png_ptr, png_ptr->chunk_name);

+   //Addition: owencqueen, 03/28/2021
+   /* Check for too-large chunk length */
+   if (png_ptr->chunk_name != png_IDAT)
+   {
+      png_alloc_size_t limit = PNG_SIZE_MAX;
+# ifdef PNG_SET_USER_LIMITS_SUPPORTED
+      if (png_ptr->user_chunk_malloc_max > 0 &&
+          png_ptr->user_chunk_malloc_max < limit)
+         limit = png_ptr->user_chunk_malloc_max;
+# elif PNG_USER_CHUNK_MALLOC_MAX > 0
+      if (PNG_USER_CHUNK_MALLOC_MAX < limit)
+         limit = PNG_USER_CHUNK_MALLOC_MAX;
+# endif  
+      if (length > limit)
+         png_chunk_error(png_ptr, "chunk data is too large");
+   }     
+
 #ifdef PNG_IO_STATE_SUPPORTED
    /* It is unspecified how many I/O calls will be performed
     * during the serialization of the chunk data.
```


### Instance 300
Here is the patch from my contribution:
```
diff --git a/DiligentTools/ThirdParty/lpng-1.6.17/pngpread.c b/DiligentTools/ThirdParty/lpng-1.6.17/pngpread.c
index 823dcad..dde7a27 100644
--- a/DiligentTools/ThirdParty/lpng-1.6.17/pngpread.c
+++ b/DiligentTools/ThirdParty/lpng-1.6.17/pngpread.c
@@ -245,6 +245,21 @@ png_push_read_chunk(png_structrp png_ptr, png_inforp info_ptr)
       if ((png_ptr->mode & PNG_AFTER_IDAT) != 0)
          png_benign_error(png_ptr, "Too many IDATs found");
    }
+   else // FIX ADDED: owencqueen, 03/28/2021
+   {
+     png_alloc_size_t limit = PNG_SIZE_MAX;
+# ifdef PNG_SET_USER_LIMITS_SUPPORTED
+       if (png_ptr->user_chunk_malloc_max > 0 &&
+         png_ptr->user_chunk_malloc_max < limit)
+         limit = png_ptr->user_chunk_malloc_max;
+# elif PNG_USER_CHUNK_MALLOC_MAX > 0
+      if (PNG_USER_CHUNK_MALLOC_MAX < limit)
+           limit = PNG_USER_CHUNK_MALLOC_MAX;
+# endif
+      if (png_ptr->push_length > limit)
+         png_chunk_error(png_ptr, "chunk data is too large");
+   }
+ 

    if (chunk_name == png_IHDR)
    {
diff --git a/DiligentTools/ThirdParty/lpng-1.6.17/pngrutil.c b/DiligentTools/ThirdParty/lpng-1.6.17/pngrutil.c
index 6c5c375..ef912e1 100644
--- a/DiligentTools/ThirdParty/lpng-1.6.17/pngrutil.c
+++ b/DiligentTools/ThirdParty/lpng-1.6.17/pngrutil.c
@@ -175,6 +175,23 @@ png_read_chunk_header(png_structrp png_ptr)
    /* Check to see if chunk name is valid. */
    png_check_chunk_name(png_ptr, png_ptr->chunk_name);

+  //Addition: owencqueen, 03/28/2021
+   /* Check for too-large chunk length */
+   if (png_ptr->chunk_name != png_IDAT)
+   {
+      png_alloc_size_t limit = PNG_SIZE_MAX;
+# ifdef PNG_SET_USER_LIMITS_SUPPORTED
+      if (png_ptr->user_chunk_malloc_max > 0 &&
+          png_ptr->user_chunk_malloc_max < limit)
+         limit = png_ptr->user_chunk_malloc_max;
+# elif PNG_USER_CHUNK_MALLOC_MAX > 0
+      if (PNG_USER_CHUNK_MALLOC_MAX < limit)
+         limit = PNG_USER_CHUNK_MALLOC_MAX;
+# endif
+      if (length > limit)
+         png_chunk_error(png_ptr, "chunk data is too large");
+   }
+
 #ifdef PNG_IO_STATE_SUPPORTED
    png_ptr->io_state = PNG_IO_READING | PNG_IO_CHUNK_DATA;
 #endif
```

## Sprint 5

### Instance 752
I have made a pull request for my contribution at: https://github.com/NoVariableGlobal/global-engine/pull/113.

### Instance 300
I have made a pull request for my contribution at: https://github.com/pcsx4emudev/DEngine-pcsx4/pull/1. 

## Sprint 6

### Instance 752
I got a response back from the maintainers of the repository. They said that they were not accepting contributions because the repository contained a university project. Therefore, I did not try further to submit this pull request.

### Instance 300
I have not yet received a response from the owner of the repository.

