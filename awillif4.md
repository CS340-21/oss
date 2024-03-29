# Sprint 1
I was assigned [ebf_stm32f407_batianhu_emwin_demo](https://github.com/Embedfire-emwin/ebf_stm32f407_batianhu_emwin_demo) and [Progression](https://github.com/LiamTyler/Progression). I looked at commit history, number of contributors, number of open/closed PR's, number of open/closed issues, and project releases to determine if the project was still in active developement.

### ebf_stm32f407_batianhu_emwin_demo Project (Instance 944)
# SP 1
This project handles PNG file processing. I determined that this project was not in active project based on the inactivity of the project. There no open or closed PR's or issues. The last commit was 7 months ago, and the only release was on April 30, 2019. Seems clear to me that this project is not in active developement.

# SP 2
This project does not seem to be accepting contributions, based on the fact that there is no documentation and only 3 contributors.

# SP 3
I conpared the files from the fix commit in libpng to the files in this project. This project contains 22 identical sets of files pngpread.c and pngrutil.c, but the files are very different from the libpng's files. Given how different these files are I am unable to determine if the vulnerability still exists.

# SP 4 and 5
I could not determine if the vulnerability existed in the code, but the project seemed to use an old version of libpng so I opened an issue explaining the possible vulnerability.
- Issue: (https://github.com/Embedfire-emwin/ebf_stm32f407_batianhu_emwin_demo/issues/1)

# SP 6
There have been no responses to the issue that I opened. I do see that another student has attempted to fix the vulnerability in one of the 22 occurrences, so I linked my issue to the [PR](https://github.com/Embedfire-emwin/ebf_stm32f407_batianhu_emwin_demo/pull/2). I cannot confirm whether the student's PR corrects the vulnerability.


### Progression Project (Instance 4)
# SP 1
This project is a C++ game engine for Linux and Windows. I determined that this project was still in active developement based on the very recent commit history, but the one contributor does not utilize PR's, issues, or releases.

# SP 2
This project also does not seem to be accepting contributions, with only one contributor and no issues, PR's, or conversations.

# SP 3
I conpared the files from the fix commit in LZ4 to the files in this project to determine that the vulnerability still exists in Progression.

# SP 4
I learned that this project was alos assigned to another student (Joey Lemon), and he has already opened a issue and provided a patch and PR.
- Issue: (https://github.com/LiamTyler/Progression/issues/1)
- Patch: (https://github.com/LiamTyler/Progression/pull/2/files)

# SP 5
Joey's PR: (https://github.com/LiamTyler/Progression/issues/1)

# SP 6
There have been no responses on Joey's PR which is still waiting for review.
