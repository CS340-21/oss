# Sprint 1

I was assigned instance 811 and 1299. I believe neither of these projects are active.

### bender647/asuswrt-382

The most recent (and only) pull request on this one is from March of last year, and it has not been accepted. This leads me to believe that this project is dead, or at least no longer accepting changes.

### zhujiadong666/PycharmWorkspace

This one returns a 404, so either has gone private or was deleted from github.

## Sprint 1 find new projets / sprint 2

Since none of these work, I've chosen instances 1028 and 1207

### DISTRHO/DISTRHO-Ports

This one seems active. There are issues that have been closed as recently as in the past month. It also seems like the project accepts contributions, as there are pull requests merged also within the last month.

### Try/Tempest

This one also seems active and accepting contributions. There are both pull requests and issues merged and closed within the past few months.

## Sprint 3

### DISTRHO/DISTRHO-Ports

This one I believe still has the vulnerability, buecause pngread.c does not contain the code that fixed the vulnerability

### Try/Tempest

This one looks like it still has the vulnerability, also because pngread.c does not contain the updated code from the the commit that fixed the vulnerability.

## Sprint 4

I fixed the vulnerability for both projects in exactly the same way: I updated pngpread.c with the relevant code. pngrutil.c did not need updating in either case.

https://github.com/sam-baumann/Tempest

https://github.com/sam-baumann/DISTRHO-Ports

## Sprint 5

Here are my pull requests

https://github.com/Try/Tempest/pull/22

https://github.com/DISTRHO/DISTRHO-Ports/pull/92

## Sprint 6

Neither of my PRs were accepted, the feedback is as follows

### Try/Tempest

In Try/Tempest, the maintainer of the repo was thankful for my PR and opted to do a full upgrade of the libpng library as opposed to patching the single file, so the vulnerability was still fixed in this case.

### DISTRHO/DISTRHO-Ports

In this repo, the maintainer explained that libpng was only used because it was part of another library used in that project, but their project does not use any libpng features so the vulnerability is not a problem for them.
