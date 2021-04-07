# Sprint 1

I reviewed the repository, commit history, issues, pull requests, and milestones to determine whether the project is still active or not. 

### Torque3D ([Instance 569](https://github.com/TorqueGameEngines/Torque3D))
**Active project.** 
There are 167 open issues and 57 closed ones. There are 15 open Pull Requests and 242 closed PRs.
The most recent PR is from 3 days agos. 
There are 4,695 commits in the history. 
Even though there are no milestones, that doesn't mean that it isn't active. Lots of groups don't use milestones. 

### Facial Recognition for Home Security System ([Instance 93](https://github.com/Mawueugiio/home))

**Project no longer active.**
There are 3 commits in the history and those were made in May 2020. 
There is also no discussion in the community, so no open/closed issues, PRs, or milestones. 
It seems that it is just a repository that stores somone's personal project to create a facial recognition system for their home that they don't plan 
on improving in the future. 


# Sprint 2 

### Torque3D ([Instance 569](https://github.com/TorqueGameEngines/Torque3D))
The project still accepts contributions as it just merged a PR 8 days ago. There are 82 total contributors listed on this project, so 
I assume that they will accept contributions as long as they were emailed about it first. First step is to get into contact with them in order to confirm
that they are allowing for more contributors. 

### Facial Recognition for Home Security System ([Instance 93](https://github.com/Mawueugiio/home))
Since the project is no longer an active project, they are not accepting contributions. There are only 2 contributors listed on this project. 

# Sprint 3

### Torque3D ([Instance 569](https://github.com/TorqueGameEngines/Torque3D))
The vulnerability referenced [here](https://github.com/glennrp/libpng/commit/347538efbdc21b8df684ebd92d37400b3ce85d55) has been addressed in [commit d0b0b4305800b640c5ae3cbc16f8c9439fc04f76](https://github.com/TorqueGameEngines/Torque3D/commit/d0b0b4305800b640c5ae3cbc16f8c9439fc04f76). This was found by searching the repository for pngrutils.c and pngpread.c and then viewing the git blame for the lines that can be seen in the referenced vulnerability commit. Viewing the git blame revealed which commit resolved the vulnerability. 

### Facial Recognition for Home Security System ([Instance 93](https://github.com/Mawueugiio/home))
The same vulnerability referenced abovve still exists in this project. They used [libpng 1.6.0 (February 14, 2013)](https://github.com/Mawueugiio/home/blob/f74ff1d14981e2d5eedfb47a3cfcb75ffa27dac1/Face_Recognition/dlib/dlib/external/libpng/pngpread.c) and the vulnerability was resolved in [libpng 1.6.37 (Aug 2, 2017)](https://github.com/glennrp/libpng/commit/347538efbdc21b8df684ebd92d37400b3ce85d55). This project was discontinued last year, so no efforts were made to resolve this issue. Both pngrutil.c and pngpread.c are in the repo, not updated due to the library version.


# Sprint 4

### Torque3D ([Instance 569](https://github.com/TorqueGameEngines/Torque3D))
This project has already implemented to patch to the libpng vulnerability referenced in Sprint 3. The commit that addresses this vulnerability patch is referenced in Sprint 3. 

### Facial Recognition for Home Security System ([Instance 93](https://github.com/Mawueugiio/home))
Since this project is very behind in the update of the libpng, the patch would be too complex to implement to address the vulnerability. It may break parts of the project itself, so it is my recommendation that the authors on this project update their libpng library to version 1.6.37 (April 15, 2019), according to the [libpng website](http://www.libpng.org/pub/png/libpng.html). 


# Sprint 5

### Torque3D ([Instance 569](https://github.com/TorqueGameEngines/Torque3D))
No patch needs to be created, so no PR. 

### Facial Recognition for Home Security System ([Instance 93](https://github.com/Mawueugiio/home))
I created an issue notifying the authors of the libpng vulnerability. Here is the [issue](https://github.com/Mawueugiio/home/issues/3). Waiting for a response. 


