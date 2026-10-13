# Processes and Signals

Bash scripting exercises covering processes and signals.

## Files

| File | Description |
|------|-------------|
| `0-what-is-my-pid` | Displays its own PID |
| `1-list_your_processes` | Lists all running processes in user-oriented format with hierarchy, using `ps auxf` |
| `2-show_your_bash_pid` | Displays lines containing `bash` from the process list, using `ps` and `grep` |
| `3-show_your_bash_pid_made_easy` | Displays PID and name of processes containing `bash`, using `pgrep` |
| `4-to_infinity_and_beyond` | Displays "To infinity and beyond" indefinitely with a 2 second sleep, using `while` |
| `5-dont_stop_me_now` | Stops the `4-to_infinity_and_beyond` process, using `kill` |
| `6-stop_me_if_you_can` | Stops the `4-to_infinity_and_beyond` process, using `pkill` |
| `7-highlander` | Displays "To infinity and beyond" indefinitely and prints "I am invincible!!!" on SIGTERM, using `trap` |
| `67-stop_me_if_you_can` | Sends SIGTERM to the `7-highlander` process, using `pkill` |
| `8-beheaded_process` | Kills the `7-highlander` process with SIGKILL, using `pkill -9` |
| `10-process_and_pid_file` | Writes its PID to `/var/run/myscript.pid`, loops indefinitely and handles SIGTERM, SIGINT and SIGQUIT, using `trap` |
| `manage_my_process` | Writes "I am alive!" to `/tmp/my_process` every 2 seconds |
| `11-manage_my_process` | Init script supporting `start`, `stop` and `restart` for `manage_my_process` |

## Usage

    ./0-what-is-my-pid

## Requirements

- Ubuntu with Bash
- First line of each script: `#!/usr/bin/env bash`
- Second line of each script: a comment explaining what it does
