# Sprint 1
I was assigned [github.com/damonyan1985/Boymue](https://github.com/damonyan1985/Boymue) and [https://github.com/ycwang812/SLAMCar](https://github.com/ycwang812/SLAMCar)

## damonyan1985/Boymue (Instance 313)

This project is surely inactive because the GitHub page has been removed entirely: the link only directs to the 404 page. As a result, I can't say for certain what the project was about or what its purpose was.

## ycwang812/SLAMCar (Instance 243)

This project is also likely inactive. The latest commit is from 11 months ago, and it was an update to the README, which only contains 1 line.

I'm guessing this project was an attempt to use the SLAM algorithms to drive a robot autonomously, as there are folders such as `PHOENIXEngine`, which are robotics libraries. SLAM is also the name of a collection of algorithms to determine the position of a robot at all times with sensory information, and is used to drive robots autonomously.

# Sprint 2

Determine if the projects still accept contributions, note the criteria you have used.

## damonyan1985/Boymue (Instance 313)

This project *definitely* does not accept contributions anymore; the entire repository has been removed from the platform.

## ycwang812/SLAMCar (Instance 243)

This project *may* accept contributions. There haven't been any pull requests to the repository, so it's hard to know for sure. The user who owns the project is active on GitHub as of March 23rd 2021, so it's likely they would see the pull request.

It's impossible to know for *sure*, but I will assume they would accept contributions.

# Sprint 3

Instance 313 does not have the vulnerability because it no longer exists, but instance 243 still definitely has the vulnerability. The files `PHOENIXEngine/PHOENIX/PX2Engine/Unity/ImageLibs/PNG/pngpread.c` and `PHOENIXEngine/PHOENIX/PX2Engine/Unity/ImageLibs/PNG/pngrutil.c` contain extremely similar code from the libpng repository, but they do not contain the added code or any comments added in the changes from [the patch commit](https://github.com/glennrp/libpng/commit/347538efbdc21b8df684ebd92d37400b3ce85d55).

# Sprint 4 & 5

Instance 313 cannot be patched because it no longer exists, but the pull request to fix instance 243 is [here](https://github.com/ycwang812/SLAMCar/pull/1). I simply [forked the project](https://github.com/adam-mcdaniel/SLAMCar), implemented the change, pushed to my copy of the repository, and created a pull request to the upstream repo.

# Sprint 6

My patch has yet to receive any responses, so I cannot reply to any messages yet.
