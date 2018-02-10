Travis reverse shell
===

Usage:

1. Generate the stty command you need with `echo stty rows $LINES columns $COLUMNS`
2. Open a listener on a machine with a public IP address with `stty raw -echo; nc -l -p 12345; stty -raw echo'
3. If you're not me, open a PR to change the name of the machine
4. Once you get a terminal, run the stty command
5. Maybe echo some stuff to /dev/fd/4 periodically to keep Travis from timing out
