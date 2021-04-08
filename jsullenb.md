I was assigned Libpng instance 478 and QEMU instance 3.  I looked at each project's commit history, open/closed pull requests and open/closed issues, and project releases to determine if the projects were still actively in developement.

Libpng (instance 478): SER401-FALL-19-Project35
This project aims to create high quality assignments of student teams.  There has not been a commit, pull request, or issue posted since April 2020, so it appears to be inactive.

QEMU (instance 3): op-tee
This is a client created that contains the TEE library for Linux.  There has not been a commit since February 2020, and there are no pull requests or issues open (I cannot tell if there were ever any in the first place, so I think it's most likely inactive.

Sprint 2
Judging based on the criteria above, it is safe to assume that both projects are not accepting contributions.  In addition, the first project seemed to be specifically for ASU students, and the second appeared to be all created by one person, so it's likely that they weren't accepting contributions even when they were active.

Sprint 3
The first project's vulnerability has not been fixed.  The vulnerability in Libpng was fixed within the last few months, about 10 months later than the most recent update to the project.  The second project's vulnerability is also out of date.  QEMU's most recent vulnerability fix was about two months ago, roughly a year since the last update to the project.

Sprint 4
The first project utilizes pngpread.c from Libpng, which was changed in the vulnerability fix.  I have applied this fix here: https://github.com/lyra3/SER401-FALL-19-Project35/blob/dev/Clique/include/fltk-1.3.5/png/pngpread.c . pngrutil.c, which was also changed in the vulnerability fix, is not used by this file.  The second project utilizes pcnet.c from QEMU, which was changed in the vulnerability fix.  I have applied the fix here: https://github.com/lyra3/op-tee/blob/master/qemu/hw/net/pcnet.c .
