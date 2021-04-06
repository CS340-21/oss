SPRINT 1
Instance #538 does not seem to be an OSS project. The most recent commits were made 7 months ago, there are no open or closed issues, and there are no pull requests.
Also, the project is in Lithuanian, which would be difficult to work with even if this was an open and active project.

Instance #1154 does appear to be an OSS project. It is an open source transportation simulation game. The repo on Github is a mirror to one located on their website
@www.simutrans.com. Commits have been made within the week. There are also pull requests, however the contributors ast that you make submissions to their forums on
their site.

SPRINT 2
Instance #1154 is still accepting contributions and submissions seem to be made rather frequently. Commits made are very recent and the project has an active forum.

SPRINT 3

Instance #1154 still contains the libpng vulnerability in the file pngpread.c. I compared the fix to the version of libpng that Simutrans was using and determined that they were not using the latest version that contained the patch. The version is recent enough that the issue can be easily resolved, simply by adding the segment of code that fixed the issue.
