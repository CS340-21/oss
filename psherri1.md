# OSS

I was assigned [Cross-platform calculator](https://github.com/Rohan-cod/cross_platform_calc) and [LZWolf](https://github.com/madmodder123/lzwolf-sdl2) as my two OSS projects.

The criteria I've used to determine if the two projeccts are still active are as follows:
- The number of participants
- Frequency of code
- Project milestones and issues
- Activity from the community, including project releases

This criteria was primarily used for sprint 1 and 2

# Cros-platform calculator (Instance #580)

## Sprint 1
This project is a calculator made using the kivy framework in python. It can be installed on mac, windows, android and ios. This project does not appear to be active. This last commit was from over 14 months ago and the last issue was assigned over a year ago.

## Sprint 2
As far as accepting contributions, this project does not appear to be doing so. There are no open discussions, pull requests, or issues fo has not had any updates for over half a year

## Sprint 3
When determining the vulnerability of the project, I compared files across the library repo and the project repo to see if the library code is present in the project than the exploit has not been fixed. I primarily looked at the pngread.c and pngutil.c files. The code mentioned in the libpng files is not present in the project so therefore it is vulnerable. For this project in particular it looks as though they are generating libpng through the use of a generated recipe, thus I do not think it is vulnerable.

## Sprint 4 & 5
Project does not seem to be vulnerable. It is generating the Libpng file by using libraries in python.
[Link](https://github.com/psherrill24/cross_platform_calc/blob/master/kivy-ios/recipes/libpng/__init__.py)

## sprint 6
No feedback given the repo is dead

# LZwolf (Instance #282)

## Sprint 1
This project is a modified game engine from the original Wolfenstein 3D engine, It combines the previous with ZDoom to create the most user and mod author friendly Wolf3D source port. This project also does not appear to be active. The last commit was over 7 months ago and has no issues or milestones.

## Sprint 2
Just like the aforementioned project, this project is not accepting any contribution through using the same criteria.

## Sprint 3
Same criteria was used as the previous project to determine if vulerability exists in the project. The code in pngread.c and pngutil.c is not in the prject's source code. It is vulnerable as well

## Sprint 4 & 5
To produce a patch for each vulnerability, I forked the project and edited the files referenced in Sprint 3 above. I encountered no issues in doing this, I also requested a pull request for it. Link is posted below.
[Link](https://github.com/madmodder123/lzwolf-sdl2/pull/1/files)

# Sprin 6
No feedback was given on the issue, repo inactive
