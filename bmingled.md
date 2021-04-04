**Sprint 1**

The two projects I have been assigned are "MVStudio" (which uses libpng) and 
"qemu" which looks like it is simply an outdated, copied over version of QEMU (which is probably why it still has the QEMU vulnerability).

*MVStudio*
- This project seems to still be somewhat active.
- The last commit as of me writing this was 13 days ago, which is fairly recent.
- There seems to be only one contributor, the main developer.
- There is not much community discussion, but there has been some in recent months.
- Based on these criteria, I would say that this project IS still active (just not super active).

*qemu*
- This project does NOT seem to be active.
- The first and last commit was made 11 months ago, which is not very recent.
- There is no community discussion whatsoever.
- Based on these criteria, I would say that this project is NOT active.



**Sprint 2**

*MVStudio*
- This project only has one contributor.
- There are no written contributing guidelines included in the repository.
- There is no pull request template.
- There is only one closed pull request, and it was from the main developer.
- For these reasons, I have concluded that the project is NOT accepting contributions.

*qemu*
- This project only has one contributor.
- There are no written contributing guidelines included in the repository.
- There is no pull request template.
- There has been only one commit ever, and it was 11 months ago.
- For these reasons, I have concluded that the project is NOT accepting contributions.



**Sprint 3**

*MVStudio*
- I looked at the commit that fixed the libpng vulnerability and compared it to the MVStudio project's file that is supposed to contain the vulnerability. 
- The changes made to the code in the libpng repository do NOT seem to be reflected in the MVStudio repository.
- Based on this and the fact that the file containing the vulnerability has NOT been updated since the vulnerability was fixed, I can confirm that the vulnerability DOES still exist in this project. 

*qemu*
- I looked at the commit that fixed the QEMU vulnerability and compared it to the 'qemu' project's file that supposedly contains the vulnerability. 
- After comparing the lines that were changed to fix the vulnerability, I can confirm that the project DOES still have the vulnerability. 
- The file containing the vulnerability has not been changed since it was fixed in the main QEMU repository.


**Sprint 4**

I decided to produce patches for both of my assigned repositories despite them both seeming to not accept contributions currently. 
I did this just as an experiment to see what would happen. To produce the patch, I corrected the two files '3rd_party/png/pngpread.c' and '3rd_party/png/pngrutil.c' in the MVStudio repository and the 'hw/net/pcnet.c' file in the qemu repository, all of which contained vulnerabilities for their respective piece of OSS. 
It was not a difficult patch as it only required changing ~20 lines of code. I did not run into any issues. I will produce pull requests for Sprint 5.


**Sprint 5**

The following are links to the pull requests I created for the patches produced.

MVStudio
https://github.com/LiangliangNan/MVStudio/pull/11

qemu
https://github.com/OneContainers/qemu/pull/1



**Sprint 6**

*MVStudio*
In a surprising turn of events, my contribution to MVStudio DID get accepted! 
The creator of the utility told me thank you for fixing the vulnerability, and that he would update the libpng library to the latest version. 
There were no issues and no further correspondence was needed to get the patch accepted.


*qemu*
Unfortunately, I never received any feedback from the owner of this repository. 
I may send a follow-up message at some point, but chances are that the owner either no longer makes use of this repository, no longer uses their Github account, or something similar, and will not probably respond. 
I will post an update here if something changes.



