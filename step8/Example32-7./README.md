# A Simple Implementation of a Progress Bar

## Description:

The main objective of the script is to display the progress bar. This script starts a background process that generates a "." every second using an infinite while True loop. When pressing ^C, the following command is triggered:
trap "echo !; kill -USR1 $pid; wait $pid" EXIT.

This command sends a SIGUSR1 signal that terminates the process with trap "exit", interrupting the infinite loop.

If you try to comment out the previously mentioned command, the loop will no longer be interrupted with ^C because SIGUSR1 will no longer receive any signal, thus requiring manual interruption via the kill command.











