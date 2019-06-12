README for the UNIX tools bk,rmb,ret
=========================


-DESCRIPTION

	This tool helps to make backups of files/folders in UNIX terminal, & retrieve them based on fileName/date/recency. FILES/FOLDERS can also be backed to a register, for a later retrieval. This UNIX tool also helps to do copy/cut/paste operation of files/folders in UNIX terminal.

See man pages of the commands for more info.


-EXAMPLE COMMANDS:

	bk <file-name>
		Backup file/folder <file-name> 

	rmb <file-name>
		Remove file/folder <file-name> after creating a backup 

	rmb <file-name> --register <register-name>
		Remove file/folder <file-name> after creating a backup in register '<register-name>' 

	ret
		Retrieve latest file/folder from backup. Equivalent to ret <file-name>

	ret --date 2d
		Retrieve all files/folders which were backed up for last 2 days. 

	ret --date 2011/10/22..2011/10/25
		Retrieve all files/folders backed up within the period 22nd to 25th Oct 2011. 

	ret --regex 'foo.*'
		Retrieve all files/folders with names starting from 'foo', from backup. 

	ret --register <register-name>
		Retrieve all files/folders in register '<register-name>', backed up. 

	ret --register <register-name> -l
		List all files/folders in register '<register-name>', backed up. 


-INSTALLATION
  	Execute install script.
		sudo ./install;


-REQUIREMENT
	LINUX/OS-X/UNIX machine with Perl 5 or above installed.

