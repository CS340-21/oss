# Sprint 1

## Criteria

I looked at the amount of open/closed pull requests and commits, as well as the latest release, amount of contributors, and the amount of issues (and whether or not the maintainers respond) to determine whether these software projects are still in development.

## libpng (instance 398)

Libpng is a library of C functions used for handling PNG images. This repository uses this code in reference to making  plugins for the synth Percussa SSP. There are no open issues or pull requests, and only appears to be one contributor, the owner of the repo. This repo seems to be soley used and maintained by one contributor (who was active from June to October of last year), since then, this repo hasn't had a commit. Based on these criteria, I determine this project to be inactive.

## qemu (instance 6)

This repo is concerned with creating a better fuzzing protocol for finding bugs/security issues in software. There are 16 contributors, but there are no issues  or pull requests listed in the repository. For my instance, there hasn't been a commit since August of 2020. There is however, a google group that appears to be active, with a steady influx of questions/patches being submitted for review. Based on this, I have determiend that this project is active

# Sprint 2

## Criteria

I looked at the amount of contributors, commit history, and checked the repository to see if there were any reference files detailing contributing the the project.

## libpng (instance 398)

This project only has commits from the owner of the repository, there are no other contributors listed, no pull requests from any other people, and no information in the reposistory about how to contribute to the repository. Based on these observations, I have determined that the project is not accepting contributions.

## qemu (instance 6)

This project has no commits or contributors listed in the repository, but it has a file claming that it is currently accepting contributions as well as a  google groups where there seem to be many active people sending in contributions (there have been 3 contributions submitted for review in the past week). Based on this criteria, I believe this project is accepting contributions.

# Sprint 3

## Criteria

I looked at the files where the vulnerability was reported to exist, as well as the reference commit that fixed the vulnerability and checked to see if my assigned repos' files had the fix in their files, if they don't, the vulnerability still exists in their project.

## libpng (instance 398)

This vulnerability involves the failure of the code to check if the data chunk size being processed is too large, this can cause issues if the data being operated on is too big. The vulnerability was fixed by adding code to check the chunk size in the pngpread.c and pngutil.c files. These files are replicated multiple times in my assigned project's repository, and none of these files have the fix. Due to this, I conclude that the vulnerbaility still exists in the project.

## qemu (instance 6)

The vulnerability involves a potential buffer overflow due to an int variable being casted to a size_t variable, the fix simply involves changing the int size variable to type size_t. The file in question, pcnet.c, does exist in my instance's repo and does not include the fix, their version of the file still has the size varibale as type int, and thus still has the buffer overflow vulnerability.

# Sprint 4

I produced patches for both of my assigned projects by forking the prject repositories and adding the code that fixes the vulnerabilities to the vulnerable files in my forked repository. The code that fixes these vulnerabilities didn't have any issues that prevented me from applying the patches, I simply added the fix to the relevant files.  These fixes are in my repo, and I will make pull requests for them on the next sprint.

# Links to patched files

## libpng (instance 398)

These files were replicated multiple times in the project repo, so I had to apply the same fix to these additional files.

Fix I applied: https://github.com/glennrp/libpng/commit/347538efbdc21b8df684ebd92d37400b3ce85d55

### pngrutil.c:



https://github.com/braymar/SSP/blob/master/technobear/rngs/JuceLibraryCode/modules/juce_graphics/image_formats/pnglib/pngrutil.c
https://github.com/braymar/SSP/blob/master/technobear/clds/JuceLibraryCode/modules/juce_graphics/image_formats/pnglib/pngrutil.c
https://github.com/braymar/SSP/blob/master/technobear/pmix/JuceLibraryCode/modules/juce_graphics/image_formats/pnglib/pngrutil.c

### pngpread.c:

https://github.com/braymar/SSP/blob/master/technobear/rngs/JuceLibraryCode/modules/juce_graphics/image_formats/pnglib/pngpread.c
https://github.com/braymar/SSP/blob/master/technobear/clds/JuceLibraryCode/modules/juce_graphics/image_formats/pnglib/pngpread.c
https://github.com/braymar/SSP/blob/master/technobear/pmix/JuceLibraryCode/modules/juce_graphics/image_formats/pnglib/pngpread.c


## qemu (instance 6)

Fix I applied: https://github.com/qemu/qemu/commit/b1d80d12c5f7ff081bb80ab4f4241d4248691192

### pcnet.c:

https://github.com/braymar/afl/blob/master/qemu_mode/qemu-2.10.0/hw/net/pcnet.c

# Sprint 5

## libpng (instance398)

https://github.com/TheTechnobear/SSP/pull/1

## qemu (instance 6)

https://github.com/CAFA1/afl/pull/1
