# Get Model, Serial Number, and BIOS Version using Command Prompt #

Use the following lines in CMD to get the model, serial number, or bios version of a device.   

**For model**

	wmic csproduct get name   
   
**For serial**

	wmic bios get serialnumber   
   
**For BIOS version**

	wmic bios get smbiosbiosversion   
