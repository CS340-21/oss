The projects I have discovered are titled [Marley](https://github.com/beaumanvienna/marley) and [Progression](https://github.com/LiamTyler/Progression).

## Sprint Criteria

### Sprint 1
My criteria to determine if they are active include exploring:
- the recency of the latest commits and issues
- the number of issues open and closed
- the number of PRs open and closed
- the project milestones and releases.

### Sprint 2
My criteria to determine if they are accepting contributions include exploring:
- the number of contributors
- the number of issues open and closed
- the activity on the issues and author responses

### Sprint 3
My criteria to determine if they still contain the listed vulnerabilities include cross-referencing the exploitable source code files between the library repo and the project repo. If the project's source does not contain the updated library code, then it is safe to assume the exploit has not been fixed.

## Marley (instance 321)

### Sprint 1
This is a bundle of gaming console emulators for the x86_64 Linux platform, licensed under the GPL-3.0 License. It stands for 
"Many Awesome Retro Linux Emulators, Yay!"

It seems to be an active project, with the latest commit on March 14, 2021 as of writing this document. It has 13 open issues, with 8 of them being opened this year
and 5 in the last week. 4 issues were solved this year. The project doesn't seem to make use of pull requests, milestones, or releases.

### Sprint 2
It also seems to be accepting contributions, with a couple of contributors and active discussions on the many open and closed issues.

### Sprint 3
The libpng exploit fix adds new code to `pngpread.c` from lines 226-240 and `pngrutil.c` from lines 184-199. However, this new code is not present in Marley at
the libpng files under the `dolphin/Externals/libpng` directory. Therefore, the exploit has not been fixed in the project.

### Sprint 4 and 5
I have raised an issue in the repository ([#86 Update Dolphin libpng library to properly check length of chunks against user limit](https://github.com/beaumanvienna/marley/issues/86)) and created a new pull request with the appropriate changes ([#87 Check length of all chunks except IDAT against user limit](https://github.com/beaumanvienna/marley/pull/87))

### Sprint 6
The pull request has been merged into the repository without any responses needed.



## Progression (instance 2)

### Sprint 1
This is a C++ game engine for Linux and Windows, licensed under the MIT License.

It also seems to be active, with the latest commit on February 13, 2021. It only has one contributor who does not make use of issues, pull requests, milestones,
or releases.

### Sprint 2
It doesn't seem to be accepting contributions, with only a single contributor and zero issues, pull requests, or discussions.

### Sprint 3
The LZ4 exploit fix adds new code to `lz4.c` at line 1043. However, this new code is not present in Progression at the `ext/lz4/lz4.c` file. Therefore, the exploit has not been fixed in the project.

### Sprint 4 and 5
I have raised an issue in the repository ([#1 Update LZ4 library to remove heap buffer overflow vulnerability](https://github.com/LiamTyler/Progression/issues/1)) and created a new pull request with the appropriate changes ([#2 Fix off-by-one error in LZ4 to fix overflow vulnerability](https://github.com/LiamTyler/Progression/pull/2)).

### Sprint 6
The pull request hasn't been responded to nor has it been merged. The repository seems to be dead.
