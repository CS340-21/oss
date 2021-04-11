# Sprint 1

I have been assigned instance 953 and instance 14. The criteria I used include the following to determine if the projects are still active: the number of participants, the frequency of the commits and issues, and the amount of discussion.

## libpng (Instance 953)
The project does not appear to be active. There are 47 participants, with only 8 different participants opening issues this year in 2021. There were also only 7 commits to the project this year as well. Also, there seem to be only a few people answering and discussing issues in the project.

## QEMU (Instance 14)
The project does appear to be active. There are 1,124 participants, with 36 commits being pushed today, March 19, 2021. There is also a separate bug report page, with around 18 users posting and answering issues this month. There also seems to be active discussion for many bug reports in this page.

# Sprint 2

The criteria I used to determine if the projects still accept contributions are commit history, the amount of contributors, and checked if there are any files that specify contribution requirements. 

## libpng(Instance 953)
The project does appear to still accept contributions. According to the recent commit history, there were 3 different contributors in the past two weeks who help find bugs in the code. I could not find any files that specify if they accept contributions, however, according to the history of the 3 contributors, they are relatively new accounts that were able to contribute.

## QEMU (Instance 14)
The project does appear to still accept contributions. However, according to the website, the instance is a read-only project and to actually contribute, you must submit a bug inquiry on their official bug report page or submit patches to the website. According to the recent commit history, there were 0 commits in the last month, but since the website does specify that "QEMU welcomes contributions of code (either fixing bugs or adding new functionality)," the project does accept to accept contributions.

# Sprint 3

In order to determine if the vulnerability still exists, I checked how the vulnerability was fixed and look to see if the code is included in my instances. If they were included, I checked to see if the vulnerability was completely solved by looking in the issues/pull requests.

## libpng(Instance 953)
The vulnerability still exists. The code to fix the vulnerability is not included in either files. Furthermore, the vulnerability fix was committed on August 2017, while my instance files' last commits were on February 2017. 

## QEMU (Instance 14)
The vulnerability still exists. The vulnerability fix was to change one of the int variables to a size_t, and according to the instance file, it is still an int. 

# Sprint 4

## libpng(Instance 953)
https://github.com/andyv0110/ebf_stm32f407_batianhu_emwin_demo/commit/ce909b92d61dcf743c11dd7ce637f13f2b6eca5d#diff-57330f18460785950d74b70aecd054bb5cafac3e3283cefddbd70b098f2eb7fb
https://github.com/andyv0110/ebf_stm32f407_batianhu_emwin_demo/commit/70e13c6404a29e12c489e6065f372b21d86c62e8#diff-a115a1321e5868ddb213fdbf08dc0f669c0e0cb908e616a9de0289f1e6d0e1b3

## QEMU (Instance 14) 
https://github.com/andyv0110/FreertosMultiUART/commit/176d0158c109419a03d3332919a30f43669f060a#diff-c63aceca62c504788add4e0228269afa4dc42db0e6f4a48d20b5cec915afa44b

While there were not any outstanding issues when producing the patches, I will note that the code in libpng(Instance 953) is significantly outdated, meaning the patch may not be utilized. 
