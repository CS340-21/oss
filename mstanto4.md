# Sprint 1
My projects are ZenonEngine(https://github.com/bouzi71/ZenonEngine) and FirmAFL(https://github.com/zyw-200/FirmAFL). In order to determine if they were active, I examined the latest commit history, number of open/closed pull requests, number of open/closed issues, and the latest project release.

### ZenonEngine Project (Instance 464)
This project is a DirectX 11 and OpenGL open source 3D enigne. 

This project seems to be an active project. However, this project only has one contributor. There is only one issue, but it is closed. There are no pull requests. The repository was last updated February 28th, 2021. There are three forks, but since there are no open or closed pull requests, it is obvious there are no other contributors. So it is not clear, if this project would accept any contributions.

### FirmAFL Project (Instance 5)
This project is a high-throughput greybox fuzzer for IoT firmware. FIRM-AFL addresses two fundamental problems in IoT fuzzing. It addresses compatiblity issues by enabling fuzzing for POSIX-compatible firmware that can be emulated in a system emulator. It also addresses the performance bottleneck caused by system-mode emulation with a technique called "augmented process emualtion."

This project does not seem to be active. It has 41 total issues, but only 10 of them are closed. There are 3 pull requests and none of them are closed. This project also only has one contibutor. It is not clear if this project would accept contributions either, since none of the pull requests have been closed. This project also does not have a commit since October 21st, 2020. 

# Sprint 2

### ZenonEngine Project (Instance 464)
There are three forks on this project, but there are no open or closed pull requests. Since there are no other contributors, it is unclear if this project would accept contributions. I do not think that it would accept contributions, but since there has not been any attempt for outside contributions, there is still a possibility that a contribution would be accepted.

### FirmAFL Project (Instance 5)
Since this project has three pull requests and none of them are closed, I would think that this project would not accept contributions. This project also does not have a commit since October 21st, 2020. Based on these characteristics of the repository, I would assume that this project would not accept contributions. 

# Sprint 3

### ZenonEngine Project (Instance 464)
The vulnerability for this project exists in the files pngpread.c and pngrutil.c in the libpng library. The vulnerability was fixed on August 2nd, 2017 in the original libpng library. This project utilizes a libpng version from May 24th, 2020. Therefore, I have concluded that this vulnerability has been fixed. The path specified by the vulnerablity was Externals/FreeImage-3.17.0/Source/LibPNG/pngpread.c and pngrutil.c which no longer exists. Having found the new source of LibPNG in path Externals/libpng, I found the link to the github version they were using for libpng, which is a newer version without the vulnerability. After talking with Dr. Mockus in class, we determined that the vulnerablity was fixed, as they were including the newer version in their library.

### FirmAFL Project (Instance 5)
The vulnerability for this project has not yet been fixed. The path to the vulnerable files are qemu_mode/DECAF_qemu_2.10/hw/net/pcnet.c and user_mode/hw/net/pcnet.c, which have not been updated to fix the vulnerablity. The vulnerability includes a possible buffer overflow exploit, which has been fixed by changing two lines of code in the pcnet.c file. These two lines have not been changed in either locations yet.
