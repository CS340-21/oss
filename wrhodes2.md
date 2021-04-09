# Sprint 1

I had the following two instances assigned
### JleMyP/game_of_life-cpp
This project I'd say is not active. Only one user makes commits, and it has no open issues/pull requests. 
The last commit was 9 months ago, and since this project is being worked by a single person 9 months since the last
(minor) commit seems quite long. Many of the commits are also in Russian (or Ukranian or some other cyrillic alphabet) 
which may pose a language barrier.

### GiantVM/QEMU
This project is also not very active, but is moreso than the previous. Only 2 contributors but does have (2) open issues
as recent as 4 months ago. 4 months ago was also the most recent commit. 

For the purposes of this assignment I'd consider the first to be inactive, while the second (giantvm/qemu) to be active enough.

# Sprint 2

Neither repo explicitly states that they're still accepting contributions, or has a contribution guide, but both allow pull requests 
and GiantVM/QEMU has open issues.

For the purposes of this assignment I'd consider GiantVM/QEMU to be likely to accept contributions while game_of_life-cpp is a toss up.

# Sprint 3

For JleMyP/game_of_life-cpp, it looks like ~~he has switched entirely from libpng to a different graphics/gui library, meaning~~ the 
vulnerability is not present at all (~~there is no pngpread.c or pngrutil.c present in the repo~~).
>*EDIT: To be more precise, this project uses the Juce library, which *does* use libpng however does not use libpng 1.6.32 which is what the patch is intended for. The libpng used here appears to be 1.6.37 which either doesn't have the vulnerability or is incompatible with the patch.*

In GiantVM/QEMU, the hw/net/pcnet.c file *is* present, as well as the vulnerability, so I will be able to produce a patch and open a pull request in subsequent sprints

# Sprint 4

I prepared a patch for the GiantVM/QEMU repo here: https://github.com/Retroville/QEMU/commit/d364048f2880e139e432238169fd88d0ecae512b

I decided not to patch JleMyP/game_of_life-cpp. See the above edit under sprint 3.

