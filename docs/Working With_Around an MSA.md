# Working With/Around an MSA #

**NOTICE:**  We are to never take a customer&#39;s Microsoft Account password. This is a breach of several policies within the company. Employee&#39;s that take Microsoft Accounts may have action taken against them of varying severity. Do NOT take Microsoft Account passwords.   
&nbsp;   
This page is guidance on how we can continue to assist the customer even if they have an attached Microsoft Account on their PC. The following options should cover most situations ranging from simple to a little tricky if they have OS corruption present.   

## Fully Functioning Machine   
 
1. **Log or Add a PIN**    
   

	You have the option to either take down the Customer&#39;s current PIN or, if they don&#39;t have one, create a PIN set to &#39;1111&#39;.   
 
2. **Create a secondary administrator**
	1. **Windows 8.1**    

		Go to **PC Settings &gt;**  click **Accounts &gt;** click **Other Accounts &gt;** click **Add an account &gt;** click **Sign in without a Microsoft account &gt;** click **Local Account** .    
&nbsp;   
The name should be something easily recognizable such as **MSStore** .    
After creating the account you need to click **Edit**  under the name **&gt;**  select **Administrator** .   
 
	2. **Windows 10**    

		Go to **Settings &gt;** click **Accounts &gt;** click **Other people &gt;** click **Add someone else to this PC &gt;** click **I don&#39;t have this person&#39;s… &gt;** click **Add a user without a Microsoft account** .   
&nbsp;   
The name should be something easily recognizable such as **MSStore** .    
After creating the account you need to click **Change account type**  under the name and select **Administrator** .   
 
## Device displaying signs of OS corruption   
 
1. **Settings app opens**    
   
	 Use the above steps to add/create a PIN or create a secondary Admin.   
 
2. **Command Prompt** (Settings app crashes or doesn&#39;t open)    
 
	There are two ways to go about this. The manual way OR the automatic way. Depending on the level of corruption the manual way may be necessary.   
 
	1. **Automatic Command Prompt account creation**    
 
		Plug in a **toolkit &gt;**  type **Win + E**  (to open File Explorer) **&gt;**  Navigate to the **toolkit &gt;**  Right click **Create MSStore Account.cmd**  and choose **Run as Administrator** .   
&nbsp;   
After the script completes you should have a secondary administrative user to use for work.   
 
	2. **Manual Command Prompt account creation**    
 
		type **Win + X &gt;**  type **A**  (to open Command Prompt (Admin))   
or   
type **Ctrl + Shift + Esc**  (to open task manager) **&gt; File &gt; Hold Ctrl**  and click **Run new task**    
or   
type **Ctrl + Alt + Del &gt; Task Manager &gt; File &gt; Hold Ctrl**  and click **Run new task**    
&nbsp;   
Then type the following into **Command Prompt** pressing Enter after each command:   

		> net user /add &quot;username&quot;   
		> net localgroup administrators &quot;username&quot; /add

		Now you should be able to log out and see another user on the login screen. Proceed with check-in.