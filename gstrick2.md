Sprint 1:

I have used the date of the last commit, amount of contributors, presence of issues and milestones, and the presence of community discussions to determine if the following projects are active. 

Algonquin - Game Dev (Instance 230)

It appears that this project is not especially active and may not be open to active contributions. The latest commit for this repo was 12 months ago. It was active January 2, 2020 to March 19, 2020. This project also appears to be in the early stages of development shown by the lack of multiple contributors and lack of previous versions of the project. The most recent version of the project is 1.0.0 which is the first release of this project. There does not seem to be any community discussion on the material present. Issues and Milestones are also not present in this repo. The only contributor to this project is floodb. Given all these factors, I would conclude that this is not an active project.

Lucmichalski/sboost (Instance 1)

This project does not appear to be very active. The last commit to this repo was 10 months ago. It appears to have only been active one day; everything was added to the repo on May 12, 2020. It does have multiple contributors which could help the probability of getting in contact with them and working collaboratively on this project. The project appears to be in early stages of development. It lacks multiple releases and versions of the project. There does not appear to be any community discussion on any of the code in the repo. Issues and Milestones are also not present. Based on all these factors, I would conclude that this project is not active. 


Sprint 2:

To see if the following projects are still accepting contributors, I looked at their commit activity on the master branch, date of the last commit, number of contributors, and the frequency of commits.

EIGHTFINITE/dolphin (Instance 11) -  This is Game cube/Wii emulator. I swapped this project with instance 230 due to inactivity and a low amount of contributors.

This project is frequently updated with new commits. It currently has 34,325 commits. Three new commits occurred today. All of them occurred at 4:00 pm today (3/23/2021) by a contributor called Eight. This project has over 451 contributors. Looking through the commit history, this project looks to be updated with commits nearly everyday. These updates include merging pull requests and updating files with features and improvements. It also appears to be updated by a different contributor each day. This project looks fairly developed but is still being updated everyday by a large pool of contributors. I would say this project would be open to accepting contributors.  

Lucmichalski/sboost (Instance 1)

This project was last updated via commit on May 12, 2020. It has 17 total commits and 2 contributors named lucmichalski and jqueguiner. Every commit was added to the repo on May 12, 2020. The repo has not been updated since. The commits appear to be merge requests and additions from 3rd parties (tag name). The number of updates appears to be split among the contributors. Since there is more than one contributor to this project but infrequent updates, I would say that this project probably would not be open to new contributors due to a loss of interest on the contributor’s part.  


Sprint 3


EIGHTFINITE/dolphin (Instance 11)

I believe the vulnerability has been patched in the pngrutil.c file for this project. I determined this by cloning the repo at the given hash (3c27fb0efaddec7821625998d294a7059f80f52f). I then cloned the libpng repo that held the commit that resolved the vulnerability. With these two repos in a directory, I then called vimdiff on both pngrutil.c in the dolphin repo and the pngrutil.c in the libpng repo. I had a difficult time finding where they fixed the vulnerability. This led me to believe that they did not fix it. I, instead, went to the repo on the github website and did a control + f on the dolphin repo in the pongrutil.c file with some of the code from the libpng commit with the fixed vulnerability. This allowed me to find where they added the patch to their code. They did not add it in the same place as the libpng pngrutil.c file did. They also updated the patch to suit their own code which could explain the small differences in code. I attempted the same method with the pngpread.c file (using the vimdiff and the control + f method) but I could not find the resolution to this vulnerability. I could not find keywords in the fixed code in the project code. This leads me to believe that they did not resolve the vulnerability in this file. As far as still being able to exploit the vulnerability, I believe that it is still possible because I cannot find where they address the variables and states in the corrected file in their own file.

Lucmichalski/sboost (Instance 1)

The vulnerability in this project was neglecting a “=” in a conditional statement. The fixed code added the “=”. I used the same method described in the above project to find if the commit, b6a35254d284deb031d90a952dd498b88eed4521, for this repo included the fixed code from the lz4 repo. I went over to the github website and used control + f, I was able to find the code using keywords in the fixed code. I found the conditional statement that the fixed code is referring to but I did not find the “=” that was added in the fixed code. This leads me to believe that the vulnerability still exists in this project. 


Sprint 4

I provided patches for the vulnerabilities described in sprint 3. By patching it, I took the code that fixed the vulnerability and added it to their code in a forked repo in my account. There were no issues experienced. The fixed code was easy to add and it didn’t appear to interfere with any of the features in the original code. I will make pull requests in the next sprint (sprint 5). Below are the links to the patched files in my forked repository for each repo. 

Patched pngread.c for dolphin: https://github.com/gstrick2/dolphin/blob/master/Externals/libpng/pngpread.c 

Forked patched for lz4.c for sboost:
https://github.com/gstrick2/sboost/blob/master/3rdparty/manticore/manticoresearch/src/lz4/lz4.c 

