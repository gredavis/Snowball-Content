# Delete Temporary Files and Settings #

**Delete IE Temporary Files and Settings**    
 
1. Open the Run box: Win + R  
2. Input one of the commands below and then press OK    
   
&nbsp;   
**Temporary Internet Files**
   
	RunDll32.exe InetCpl.cpl,ClearMyTracksByProcess 8   
&nbsp;   
**Cookies**

	RunDll32.exe InetCpl.cpl,ClearMyTracksByProcess 2   
&nbsp;   
**History**

	RunDll32.exe InetCpl.cpl,ClearMyTracksByProcess 1   
&nbsp;   
**Form Data**

	RunDll32.exe InetCpl.cpl,ClearMyTracksByProcess 16   
&nbsp;   
**Passwords**

	RunDll32.exe InetCpl.cpl,ClearMyTracksByProcess 32   
&nbsp;   
**Delete All**

	RunDll32.exe InetCpl.cpl,ClearMyTracksByProcess 255   
&nbsp;   
**Delete All - &quot;Also delete files and settings stored by add-ons&quot;**
  
	RunDll32.exe InetCpl.cpl,ClearMyTracksByProcess 4351

&nbsp;

**Ctrl + shift + Del while in IE.**

&nbsp;