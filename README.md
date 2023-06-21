# PClub_Secy_Task-4
I started by testing the maximum string length that can be inputted into the chat. It turned out to be 1000 characters long. I tried inputting more than this, but I got an error message. Then I used inspect element to see the error when inputting more than 1000 characters. 
I get the following error : 
{'content': [ErrorDetail(string='Ensure this field has no more than 1000 characters.', code='max_length')]}

Unable to proceed further this way. I tried to use cmd to SSH with the site and failed. I tried curl and tried sending a file but got no interesting output.
I read a few papers online on buffer overflow susceptibility and exploitation. I also saw videos online on how to exploit such an error. I learnt that usually, such inputs are stored in a randomly allocated memory location in the stack. Now if you input more than the memory space allocated to this, it may "overflow" into adjacent memory and corrupt that data. Hackers use this part, the part overflows into the unwanted region, to inject some code that can grant them access to protected data, etc. I tried emulating their steps but was unable to proceed. In the end, I hit a brick wall. But if i was given more time, I think that I could have made some significant progress. 
