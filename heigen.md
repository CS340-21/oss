# Sprint 1

### Sauce3D (instance 911)
This is a 3d rendering engine for a larger graphics engine project.
This project is not active. The last commit was nearly a year ago and there are no issues. In addition, there are no forks being developed. 
Github lists no dependants using this project, so it is of no interest to anyone other than the sole contributer who has stopped working on it.

### amiga-utils (instance 996)
This is an Amiga project for assembly.
This project seems to be in active development. It has had steady commits for several years.

# Sprint 2

### Sauce3D (instance 911)

There are no pull requests, forks, or issues. The creator is the sole contributor. The creator has only had activity on Github twice in the last year, so even if he/she were open to contributions, it's unknown whether they will log on to see them.

### amiga-utils (instance 996)

There are no pull requests or forks. I did see one issue asking about the license, so it seems like the project might be used by someone outside of the creator. The creator is the sole contributor, however he/she is relatively active on github, so they might be open to contributions. 

# Sprint 3

### Sauce3D (911) & amiga-utils (996)

In both cases, the files in question had been updated since the libpng commit. However, I was unable to find some code from that commit in either of the files. This prompted me to look at the libpng's pngpread.c file. The source file doesn't contain the code either, so I'm guessing they've subsequently changed things further. I am not sure how to check whether the vulnerabilty remains, however I would be surprised if it didn't, given that the projects seem up to date with the current libpng repo.

# Sprint 4

The links to my patches are below. I didn't have any issues.

### Sauce3D (911)

pngpread.c: https://github.com/bitsauce/Sauce3D/commit/668c58627e0e8b092004be91f917d5718ad238d1
pngrutil.c: https://github.com/bitsauce/Sauce3D/commit/56c099b883b118b924d81a4478c2a429b437757f

### aminga-utils (996)

pngpread.c: https://github.com/skeetor/amiga-utils/commit/9554281fbe36f46a11a45d55317ede3cb18c3a1c
pngrutil.c: https://github.com/skeetor/amiga-utils/commit/e9572ba75c9f70b22235ac2faaecce11b5ebf4c9



