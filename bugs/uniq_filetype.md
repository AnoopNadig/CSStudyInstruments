## Meta
* Project: uniq
* Project Bug Identifier: 
* Link to Bug on Project Bug Tracker: 
* Current Stage: 
* Brief description (This can change as you progress) :

The command 'uniq' does not throw an error when the filetype of input is changed to a block device.


## Updates


### Week 1

**Current Stage: Bug Identified**

A bug was discovered when using crash simulator on the command uniq.
The rreplay showed that an fstat accepted block device file type input.
The command did not perform a check when passing a block device file type as an input. 

### Week 2

**Current Stage: Bug Identified**

Experimented more with the utility for other file types as input. After discussing with Preston concluded that the utility accepting block and character devices without performing any checks is indeed a bug. 

### Week 3

**Current Stage: Bug Identified**

I was unable to work on this bug.

### Week 4

**Current Stage: Source of Bug Diagnosed**

Reviewing the source code revealed that the problem exists because the current implementation of the internal function freopen() does not check for the file type being passed as an input. Begun investigating ways to perform the required check.

### Week 5

**Current Stage: Bug Fix Implemented and Bug Fix Submitted to Project**

Used the function stat() to perform the required check for character and block type devices. After creating a patch for it tested it to make sure it doesn't break any tests. Finally, reported the bug to Ubuntu's launchpad according to project standards and also uploaded the patch. Here's the link: https://bugs.launchpad.net/ubuntu/+source/coreutils/+bug/1808095
