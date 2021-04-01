I was assigned Instance 817(86U-merlin) and Instance 3(DIR882A1-GPL).

Sprint 1:

86u-merlin is a software for products related to ASUS wireless routers. It seems fairly inactive. It's been 4 months since the last commit and there are only 21 commits.

DIR882A1-GPL is a code dump for a DLINK product. It is inactive. There are only 5 commits and they were all on the same day over a year ago.

Sprint 2:

86u-merlin does not seem to be open to contributions. All 21 commits are from the same person.

DIR882A1-GPL also isn't open to contributions. All commits were on the same day and by the same person.

Sprint 3:

The vulnerability exists in pngread.c and pngrutil.c and was fixed in 2017. 86u-merlin uses a version of pngread.c from 2010, so the vulnerability does still exist in this program.

The vulnerability exists in http_auth.c and mod-auth.t. Upon inspecting these files in DIR882A1-GPL, they don't contain the fixes that were pushed to Lighttpd in 2011, so the vulnerability still exists.
