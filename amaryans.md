
For this I was assigned instance 1247 - stepmania/stepmania

Sprint 1
This project seems to be open and relatively active as there have been pull requests made in the last year as well as commits as recently as 2 months ago. The project is not incredibly active as there are 110 contributers and so few commits, but it is still being revised

Sprint 2
Based on the fact that there are many contributors and the project is slowly making progress (last commit was 2 months ago) we can assume that it is still accepting contributions, but the continuation of the project does not seem to be a priority.

Sprint 3

This project is currently using the version of libpng from 2019, and since the vulnerability was patched in the 2017 version, the patch has been fixed.

Sprint 4/5
Since the vulnerability has been addressed in the 2019 version, there is no reason the address this with a new patch

For this I was also assigned instance 364 - Totalcross/totalcross

Sprint 6
No need for PR since patch was there already

Sprint 1
This projects is still active, and there have been commits made withing the last 7 days. There are only 15 contributors but with 8 recent pull requests we can see that this project is indeed active. 

Sprint 2
This project does seem to be accepting contributions considering there are only two PRs open from last year, and with commits being made so recently it is very active. 

Sprint 3

After investigation of the libpng libraries, this project is using an older version (2016) of the libraries which still contain the vulnerability, this project is still vulnerable.

Sprint 4/5
Forked the project and changed both of the files described above with the vulnerability patches. Links to the changed files are below. Since I am not a part of the organization that is working on TotalCross, I am not allowed to make a PR. I have made a PR on my own fork though if that is acceptable. If not let me know and I will attempt to join their project and submit the request.
https://github.com/amaryans/totalcross/blob/amaryans-patch-1-pngpread-vulnerability/TotalCrossVM/src/png/pngpread.c
https://github.com/amaryans/totalcross/blob/amaryans-patch-2-chunk-length-vulnerability/TotalCrossVM/src/png/pngrutil.c

Sprint 6

Unable to get changes to repo merged because of PR criteria of the repo.
