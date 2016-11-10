# Rebuild BCD (Boot) #

The following will create a backup of the current boot record and create a new one using recovery media.<br>
This is useful for "my PC updated and now it doesn't boot" problems, amongst others.<br> Press **Enter** after entering each of the following lines.   

`bootrec /rebuildbcd` -- add installations if available --<br>

`bcdedit /export c:\bcdbackup`<br>

`attrib c:\boot\bcd -h -r -s`<br>

`ren c:\boot\bcd bcd.old`<br>

`bootrec /rebuildbcd` --select or deselect as necessary --   
   
Additionally, you can run
	`bootrec /scanos`
to see if there is even a Windows directory found on the HDD.   
   
You can also run `bootrec /fixboot` to attempt to automatically repair boot issues.   

Finally, you may be able to run `bootrec /fixmbr` as a last attempt.