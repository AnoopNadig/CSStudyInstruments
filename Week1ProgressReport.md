* Started working with Crash Simulator. Initially spent quite a lot of time trying to set it up but finally started using Alex's image.
* Used Crashsim on three utilities: uniq, chown and hostname
  * uniq: Observed that the command accepted all the file types and wasn't able to handle the device file urandom. Preston also advised and confirmed that this was indeed weird behavior and may be a potential bug.
  * chown and hostname: Faced issues when trying to create tests for this command so kept troubleshooting.
* While experimenting with the tool observed a few discrepancies and raised two issues:
  * [rreplay fails when the "trace_snip.strace" file contains "exit_group(0"](https://github.com/pkmoore/rrapper/issues/37)
  * [rreplay fails when number of lines are less than the default value in "trace_snip.strace" file](https://github.com/pkmoore/rrapper/issues/38)
