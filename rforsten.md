The two projects I was assigned are RafaleSoft/Raptor and xiangshouding/gyp. Neither of these projects have very detailed README files, so it is difficult to understand the purpose of each.

Milestone 1:  
For determining whether each project is still active, I have looked through the main metrics of a github project: issues, commits, pull requests, and milestones. Within each of these categories, I checked both the quantity and recency of the content.

RafaleSoft/Raptor  
This project seems like it may still be active to a degree. It currently has 6 issues open and 1 closed. However, all of these issues date back at least a year and some multiple years, so it does not seem like the issues have been closed when they are finished. Unlike the issues, the commits for this project are much higher in quantity and recency. The project has nearly 500 commits with the most recent being January 17th, 2021. Currently the project has no pull requests or milestones, but this may be due to the low number of contributors. 

xiangshouding/gyp  
This project looks like it is not still active. Their are only 36 commits, the last of which was 10 months ago. Before that the project had not been touched since 2017. It only has 1 issue currently open from 2019 and it seemed to be more of a discussion than anything else. The project also has no pull requests or milestones. The last closed pull request was from 2016. 

Milestone 2:  
For determining whether each project is still accepting contributors the main factors I have looked at are the number of contributors, the number of commits, and the recency of the commits. 

RafaleSoft/Raptor  
It does not seem like this project is really accepting contributions from anyone, or at the least, it has not in the past. The project only has two contributors, both of which have been making contributions throughout the lifetime of the project. Both of these contributors still seem to make commits frequently and recently, but most of the issues for the project are seemingly outdated. 

xiangshouding/gyp  
Similar to the other project, this one does not seem to be accepting contributions either. Beyond the fact that the project does seem to be active still in general, it has only had 2 contributors in its lifetime. The project does have 5 forks, but after checking each of these as well, none of them have been changed in 4 to 6 years. 


Milestone 3:
For determining whether or not the vulnerability still exists, I have cross referenced the commit that fixed the vulnerability in the libpng library with the source code of the two projects. The commit to fix the vulnerability altered two files in the library: pngpread.c and pngrutil.c.

RafaleSoft/Raptor  
File locations: Raptor/AddOns/libpng-1.6.36/source/pngpread.c and pngrutil.c  
Neither of the two files have the necessary updated code to fix the vulnerability. 

xiangshouding/gyp  
File locations: gyp/third-party/libpng/pngpread.c and pngrutil.c 
Neither of the two files have the necessary updated code to fix the vulnerability. 


Milestone 4 and 5:  
RafaleSoft/Raptor: https://github.com/RafaleSoft/Raptor/pull/12

xiangshouding/gyp: https://github.com/xiangshouding/gyp/pull/6


Milestone 6:  
Neither one of the repositories have accepted the merge, but I do not believe they will since they have both been inactive for some time. I provided links explaining the exploit, as well as a link to the commit that fixed the exploit in the libpng library for both pull requests. 
