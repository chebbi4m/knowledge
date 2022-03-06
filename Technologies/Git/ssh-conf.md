# Generating a new SSH key

1. Open Git Bash.

2. Paste the text below, substituting in your GitHub email address:
   	```
	$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com" 
	```
3. press Enter. This accepts the default file location.
4. type a secure passphrase (!!! it's a password save it !!! )
5. Adding your SSH key to the ssh-agent :
   	```
	$ eval "$(ssh-agent -s)" 
	```
6. Add your SSH private key to the ssh-agent
   	```
	$ ssh-add /c/Users/<username>/.ssh/id_rsa // For Windows
	$ ssh-add /home/<username>/.ssh/id_rsa // For Linux  
	```
* <b>when you create the ssh key it tells you to choose the path, thats the defauls path.
	If you change the default path, put the new path you chose.</b>

7. Add the SSH key to your account on GitHub. (id_rsa) (you will find the file in .ssh file)
	
	<b>In github, under profile > settings > SSH and GPG keys</b>
    	
	```
	Title: <Your_OS>
    	key: paste the full content of id_rsa
	```  
8. YOU DID IT :D You added the ssh configuration to your project

### <i> ( If you close the terminal repeat steps 5-6 ) </i>
