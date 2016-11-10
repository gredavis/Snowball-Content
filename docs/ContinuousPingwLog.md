## Continuous ping with log

An easy way to check for intermittent wireless issues is to run a ping test and have it save to a log.   
 
1. Open Command Prompt with Admin  
2. Enter the following command and press Enter    
  
		ping bing.com > c:\pingtest.txt -t 
 
3. It is now constantly pinging the website you specified. It may appear inactive while running but you can verify the activity by navigating to C:\pingtest.txt. You can open this .txt at any time during the process to verify activity.    

To stop running the continuous ping command simply press Ctrl + C in the command prompt window. You can now verify the final version of the log in C:\pingtest.txt.