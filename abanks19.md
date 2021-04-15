# **Sprint 1**

I was assigned Libpng and Lighttpd. I looked at the commit history, open/closed pull requests and open/closed issues, and project releases to determine if the project 
was still in active developement.

### ProjetKF Project (Instance 55)
The project's goal was to create a software able to animate a 3D mesh with live recorded facial expressions.

Judging by the fact that there has not been a commit in 11 months and there are no pull requests or issues, I'd say the project is not active.
### DIR882A1-GPL Project (Instance 1)
There is no file that acutally describes what this project is. It is just several dozen code files with no comments.

Every file was commited on January 2nd 2020 by one author along with a single release. It does not seem like this project was ever active, the author seemed to use github to store a personal product that they have no intention of updating.

# **Sprint 2**

Using the above criteria, it would appear that neither of the projects are excepting new contributions.

# **Sprint 3**

I appears that both projects have not fixed their vulnerability. I have determined this by looking at the committ that repaired the vulnerablility in libpng and lightpad and comparing it against the most recent committ for both projects. Both are running older versions of the code with the vulnerabilities still intact.

# **Sprint 4**
### ProjetKF Project (Instance 55) Patch
  https://github.com/Andrew-Banks-UT/ProjetKF/blob/master/dependencies/dlib-19.19/dlib/external/libpng/pngrutil.c
  https://github.com/Andrew-Banks-UT/ProjetKF/blob/master/dependencies/dlib-19.19/dlib/external/libpng/pngpread.c

### DIR882A1-GPL Project (Instance 1) Patch
  https://github.com/Andrew-Banks-UT/DIR882A1-GPL/blob/master/user/tw-prog.priv/lighttpd_mtk/lighttpd-1.4.20/src/http_auth.c
  
No issues patching either code. 

# **Sprint 5**
https://github.com/khaledabdrabo98/ProjetKF/pull/1
https://github.com/ljrk0/DIR882A1-GPL/pull/2
