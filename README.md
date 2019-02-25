Using the List User Repositories Github REST API, write a program to return the list of public repositories accessible to my user account. 

Steps:

# 1. Install jq

   You can use
   ```$ brew install jq```
	
   if you are using Mac. 
    
   For Windows users, if you have "choco" (https://chocolatey.org), the following should install a pre-compiled binary:
    ```choco install jq```
	 
# 2. Use Terminal or Bash to get the list of public repositories ##

  Download CURL if you don't have it installed. 
  ```https://curl.haxx.se/download.html```

  After you successfully installed CURL and JQ, input following code in bash or terminal to get my public repositories.
  
	```curl "https://api.github.com/users/LaisiMa/repos?per_page=100&page=1" | jq -r '.[] | .name';```
  Thank you!

