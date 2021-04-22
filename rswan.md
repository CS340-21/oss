SPRINT 1:

For this project I was assigned, Libpng, a graphics library, and QEMU, a machine and userspace emulator and virtualizer. Libpng does not seem to be very active with almost everything in the repository not being updated in the last year, but QEMU does seem active with many commits in the last week. 

Libpng (Instance 1211)
This instance has to do with the chromium web browser and I concluded that this branch of the project is no longer active. There are no open issues and the most recent commit was 12 months ago. From what I could tell this project is inactive.

QEMU (Instance 1)
This instance appears to be an early version of the project and seems to have been resolved around a year or more ago. The most recent commits on this instance come from 12 months ago. These are no open issues so I believe this project is inactive.


SPRINT 2:

Libpng (Instance 1211)
This project has not had a successful commit in the last 12 months. Also there are three pending pull requests two from the beginning of January and one from 6 days ago. Since these have not been accepted I concluded that this project is not accepting new commits at this time.


QEMU (Instance 1)
This project has no active issues or pull requests and the most recent commit was 13 months ago. From this I have concluded that this project is likely not accepting any new commits at this time.


SPRINT 3:

Libpng (Instance 1211)
To check if this vulnerability still exists I checked the commit that fixed the LibPNG vulnerability and compared it to the files that contained the vulnerability. These two files were pngrutil.c and pngpread.c. Both of the files in the instance I was tasked with do not contain the code that was added to fix the vulnerability. Based on this I have concluded that the vulnerability still exists in the project. 

QEMU (Instance 1)
To check if this vulnerability still exists I checked the commit that fixed the QEMU vulnerability and compared it to the file that contained the vulnerability. The file that contained the vulnerability was pcnet.c. The file in the instance I was tasked with does not contain the code that fixed the vulnerability. Based on this I have concluded that the vulnerability still exists in the project. 

SPRINT 4:

Libpng (Instance 1211)
To fix this vulnerability I copied the code from the commit that fixed the issue into the file that contained the vulnerability The link to my updated file is below.
https://github.com/BuddySwan/chromium/blob/master/third_party/libpng/pngpread.c
https://github.com/BuddySwan/chromium/blob/master/third_party/libpng/pngrutil.c

QEMU (Instance 1)
To fix this vulnerability I performed the same action as I did for the vulnerability in Libpng. The link is below
https://github.com/BuddySwan/qemu-2.10.0/blob/master/hw/net/pcnet.c

SPRINT 5:

I created pull requests for both of the fixes made in Sprint 4

Libpng (Instance 1211)
https://github.com/ECS-251-W2020/chromium/pull/5

QEMU (Instance 1)
https://github.com/ssdemajia/qemu-2.10.0/pull/1

SPRINT 6:

Neither pull request has had any activity so there is nothing to report on.


