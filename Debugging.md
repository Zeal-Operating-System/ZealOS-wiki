## Debugger
The system Debugger can be invoked by calling `Debug;`, pressing `Ctrl-Alt-D`, or is entered during faults. It is a command line interface, just like the rest of the OS. You can enter `Help;` at the debug command line to get a summary of some helpful functions.

When editing files in the Debugger, it uses EdLite instead of Ed. Both editors work the same, and have the same keybindings.

The debugger pauses code execution, leaving registers, stack, and compiler information as-is. You can modify all of these from the debugger. The current register state gets printed to the top right corner of the screen.

See [Doc/DebugOverview.DD](https://zeal-operating-system.github.io/ZealOS/Doc/DebugOverview.DD.html) for more advanced info.

## Debugging Functions
There are a wide variety of debugging functions. Depending on what issues you're facing, certain functions may be more useful than others. They can be used everywhere, not only when in Debug mode. This is not a full list, just some more common debugging functions.

* `Man` - Jumps to the source code of a function. Example: `Man("KMain");`
* `E` - Jumps to source code of a function, arg is function address with offset. Example: `E(&Lex+0x0C11);`
* `Fix` - Jumps to line number & file where error occurred. 
* `CallerRep` - Report calling routines.
* `StackRep` - Report what's on the stack.
* `Prof` - Start the code profiler. Useful for trying to figure out where CPU time is spent.
* `ProfRep` - Stop the code profiler and report the profiling data.
* `Uf` - Unassemble a function, print the assembly code. Example: `Uf("Print");`
* `FunRep` - Show names and values of a function's local variables. Example: `FunRep("MountFile");`
* `ClassRep` - Reports class data, takes argument as a pointer. Example: `ClassRep(&blkdev);`
* `B2` - Clear all breakpoints.
* `S` - Single-step.
* `G` - Resume execution.
* `G2` - Clear all breakpoints, flush screen framebuffer, focus window, resume execution.
* `Exit` - Kill current task.

## Troubleshooting
* To stop a program during execution, add a call to `Debug;` to enter the debugger, or `throw;` to halt program execution. `throw` can take an integer error code as an argument: `throw(-1);` or `throw('error');` for example.