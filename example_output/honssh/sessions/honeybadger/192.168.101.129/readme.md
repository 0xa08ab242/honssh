# SAMPLES from the SESSIONS directory

### Background
other than this readme file, the directory and contents were created by a simple test instance of honssh

### 20150823_181405_919417.log
file name indicates date and time
	YYYYMMDD_hhmmss_subseconds.log
log data showing on different lines with date-time of each entry, examples include
	(honeypot assigned name, IP address and listening port)
	(incoming connection data - source IP, source port, SSH client version information)
	(open terminal channel, i.e. shell)
	(terminal commands executed)
	(close terminal channel)
	(close SSH connection)
	
### 20150823_181405_919417.tty
log of the actual session from the login banner to the logout
	viewable in a hex editor as well as the provided kippo (which I have not yet attempted to use)
	a cursory review with said hex editor reveals that most of the data is in human readable text
		looking for other (possibly standalone) options to play back the data on Windows
			termrec https://github.com/kilobyte/termrec) shows a little, but is still not suitable
	might be useful to write a script to parse the file for consumption by other applications
		hubot comes to mind...  I need to think about this a bit (plus this is a lesser priority at the moment)