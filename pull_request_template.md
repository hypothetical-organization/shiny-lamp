This new branch essentially contains a new file to contain msgs for command ingest 2 along with the msgids for the app

## Description\
There is a file called cmd_ingest_2_msgs.h which contains the structs for the new command ingest 2 messages. In moonranger_msgids.h there are several msgids added in for the app

This was required so the new command ingest 2 app would work thus creating functionality for communication with the iOBC.

## How has this been tested?
Unit tests have been created and it was built alongside the other apps.

I tested it in a docker container within ubuntu

It should not affect other areas of the code

## Screenshots (if appropriate):
Types of changes\
[] Bug fix (non-breaking change which fixes an issue)\
[x] New feature (non-breaking change which adds functionality)\
[] Breaking change (fix or feature that would cause existing functionality to not work as expected)\


##Checklist:\
[] I have read and followed the CONTRIBUTING.md file\
[x] I have applied the .clang-format file to my changes\
[x] I have commented my code using Doxygen style comments (see Contributing MD for examples), particularly in hard-to-understand areas\
[x]I have made corresponding changes to the design documentation\
[x]I have updated any relevant parameters in the internal ICD\
[x] My changes generate no new warnings\
[x] I have added tests that prove my fix is effective or that my feature works\
[x]If this is a bug-fix, I have added tests that can catch similar bugs in the future\
[x] New and existing unit tests pass locally with my changes\
[x] For cfe apps I have reserved an empty address for my msgs_ids and perf_ids from the tracking list and checked that it does not clash with other apps\
[x] For new added message types, there is a timestamp included via either an explicit timestamp variable in the struct or buried in the a tlmHeader.\
