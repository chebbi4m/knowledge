Initial repository remote :  step by step
## CASE OF NEW REMOTE REPOSITORY
## CASE OF EXISTING REPOSITORY

# CASE OF NEW REMOTE REPOSITORY 

1. Create the repository on the remote server ('GitHub.com')


2. Create local Repository:
	```
	Just create a local directory in a path of your own choosing
	```
3. Open the local Repository on the command line:
	```
	// Command line: *git bash
		         *powershell
	// Place yourself into that directory with "cd <path>" command
	```

4. Intiate a local git repository:
	```
	$ git init
	```

5. Change the default branch from master to main:
	```
	$ git branch -M main
	```

6. Link the remote repository to local repository:
	```
	// git remote add <name> <url>
	$ git remote admin git@github.com:FaroukBousselmi/Orion-Sen_Admin.git
	```

7. Create a README file:
	```
	// This command will create the file 
	// touch <file-name>
	$ touch README.md


	// This command will write a message in the file
	// echo "<message>" >> <file-name>
	$ echo "description" >> README.md

	// Don't forget the file extention (.md /  .txt / ...)
	```
8. Track files with git:
	```
	// this command will put all the files in current directory under git tracking 
		$ git add * // Add all the modified files to the staging area 
	// Or use this to add specific filegit add <file>
	```
9. Save changes <b>locally</b>:
	```
	$ git commit -m "<message>"      
	// The message is brief info about the commit
	```
10. Save changes to the remote server:
	``` 
	// Command : git push -u <name> <branch>
	$ git push -u admin main
	```
</br>
</br>

# CASE OF EXISTING REPOSITORY 


1. Create local Repository: 			
	
	```
        Just create a local directory in a path of your own choosing
        ```
2. Open the local Repository on the command line
	```
	// Command line: *git bash
	    	        *powershell
	// Place yourself into that directory with "cd <path>" command
	```

3. Intiate repository
	```
	$ git init
	```

4. Change default branch master to main :
	```
	$ git branch -M main
	```

5. Link the remote to local repository
	```
	$ git remote add <name> <url>
	// Example : git remote add admin git@github.com:FaroukBousselmi/Orion-Sen_Admin.git
	```
6. Create a README file :
	```
	// This command will create the file :>touch <file-name>
	$ touch README.md


	// This command will write a message in the file :echo "<message>" >> <file-name>
	$ echo "description" >> README.md

	// Don't forget the file extention (.md /  .txt / ...)
	```
7. Track files with git :
	```
	// This command will put all the files in current directory 
	under git tracking (Staging area)
	$ git add * 
	// Choose the file you wanna track 
	$ git add <file>
	```
8. Save changes locally :
	```
	$ git commit -m "<message>"      
	// The message is brief info about the commit
	```
9. Save changes to the remote server :
	``` 
	$ git push -u <name> <branch>
	// Example : git push -u admin main
	```
