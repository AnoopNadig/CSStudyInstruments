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
