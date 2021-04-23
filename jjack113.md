# Sprint 1
My projects are opencv (https://github.com/opencv/opencv) and Qt5 (https://github.com/CdTCzech/Qt5). 
I examined the commit history, the number of open and closed pull requests, and the number of open and
closed issues, contributors, and the latest project release to determine if the project was active. 

### opencv (instance 1337)
When I reviewed this project, it had been updated 20 minutes prior. It has 78 pull requests, all of which are
open. It has 1,861 open issues and 5,975 closed issues. There are also 30,240 commits and the lastest project 
release was December 20, 2020. There are a total of 1,296 contributors. From this information, I have concluded 
that this is an open and active project. 

### Qt5 (instance 1319)
The last commit to this project was February 11. It only has 3 pull requests, but all three are open. It has no 
issues. There are a total of 12 commits, all from a single person, so I assume that person is the only 
contributor. There is no date for the latest project release. From this information, I have concluded that this is
and open and active project. 

# Sprint 2

### opencv (instance 1337)
There are already a total of 1,296 contributors and the last commit was 11 hours ago. There are 79 open pull requests 
and 11,783 closed pull requests. Between March 16, 2021 and March 23, 2021, there have been 17 active pull requests--12 merged
pull requests and 5 open. From this information, I would conclude that this project is still accepting contributions. 

### Qt5 (instance 1319)
There have been 2 open pulls requestes February 23, 2021 – March 23, 2021. In total, there are 5 open pull requests and 
2 closed pull requests. So far, there appears to be only one contributor. However, I believe there is a chance that 
this project would still accept contributions, for it seems to only be checked on and altered periodically (I based
this on the commits/contributors graph found under the insights tab. 

# Sprint 3

### opencv (instance 1337)
The first thing I did was open the commit where the vulnerabilities in files pngpread.c and pngrutil.c were fixed so I could 
determine what code I needed to look for within the project's files. I then opened the project, followed the path 
'3rdparty/libpng/pngpread.c and pngrutil.c', and viewed the files. I did not find the specific chunk of code that was referenced 
in the vulnerability-fix commit in either of the files, leading me to believe that the vulnerability still exists. 

### Qt5 (instance 1319)
The first thing I did was open the commit where the vulnerabilities in files pngpread.c and pngrutil.c were fixed so I could 
determine what code I needed to look for within the project's files. I then opened the project, followed the paths 
'qtwebengine/src/3rdparty/chromium/third_party/libpng/pngpread.c and pngrutil.c' and 'qtwebengine/src/3rdparty/chromium/third_party/pdfium/third_party/libpng16/pngpread.c and pngrutil.c', 
and viewed the files. I did not find the specific chunk of code that was referenced 
in the vulnerability-fix commit in either of the files from either path, leading me to believe that the vulnerability still exists. 

# Sprint 4/Sprint 5

### opencv (instance 1337)
I edited the files pngpread.c and pngrutil.c (found in the path mentioned above) and inserted the correct code fragments as specified 
in the commit https://github.com/glennrp/libpng/commit/347538efbdc21b8df684ebd92d37400b3ce85d55. I then created a pull request and explained 
in a comment the edits I made, as well as linked the commit that fixed the vulnerabilities: "Check length of all chunks except IDAT against user limit". 
Here is a link to my pull request: 

https://github.com/opencv/opencv/pull/19878

### Qt5 (instance 1319)
I edited the files pngpread.c and pngrutil.c (found in the paths mentioned above) and inserted the correct code fragments as specified 
in the commit https://github.com/glennrp/libpng/commit/347538efbdc21b8df684ebd92d37400b3ce85d55. I then created a pull request and explained 
in a comment the edits I made, as well as linked the commit that fixed the vulnerabilities: "Check length of all chunks except IDAT against user limit". 
Here is a link to my pull request: 

https://github.com/CdTCzech/Qt5/pull/14

# Sprint 6: 

### opencv (instance 1337)
I received a response from an administrator on my pull request for this project and it turns out the I misinterpreted the code and there is no vulnerability, meaning a patch was not necessary. The following was the response from Alexander Alekhin: 

"These patches are against 1.6.31+
Current code is based on libpng 1.6.37

Refer to the content of the latest libpng release: https://github.com/glennrp/libpng/tree/v1.6.37
There are no such workarounds anymore, probably they are mitigated through different ways."

He then closed the pull request. 

This is the citeria for a good pul request as specified by the opencv admins: 

"Pull Request Readiness Checklist
See details at https://github.com/opencv/opencv/wiki/How_to_contribute#making-a-good-pull-request

 I agree to contribute to the project under Apache 2 License.
 To the best of my knowledge, the proposed patch is not based on a code under GPL or other license that is incompatible with OpenCV
 The PR is proposed to proper branch
 There is reference to original bug report and related work
 There is accuracy test, performance test and test data in opencv_extra repository, if applicable Patch to opencv_extra has the same branch name.
 The feature is well documented and sample code can be built with the project CMake"
 
### Qt5 (instance 1319)
I did not receive a response on this project, so it is likely not an active project after all. Nevertheless, I realized that I made the same mistake 
as I did in the opencv project and a patch was not necessary. I commented "I made a mistake and no patch is necessary. My apologies." and then closed the 
pull request. 
