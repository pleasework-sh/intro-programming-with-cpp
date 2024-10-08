# Creating and cloning your GitHub repository
If you are not logged in already, go to github.com and log in.

To your left, click on the green "New" button.
![text](../../image/6-creating-and-cloning-your-repo.png)

Name the repository "CSC114-Fall2024", add a description, set the visibility to "Private" and add a README.md file.

Scroll down and click "Create Repository".

![text](image/6-creating-and-cloning-your-repo-1.png)

![text](image/6-creating-and-cloning-your-repo-2.png)


# Share the file with your instructor
On the next page, click "Settings".

![text](image/6-creating-and-cloning-your-repo-3.png)

On the lefthand menu, click "Collaborators" and then follow the authentication prompts. 
![text](image/6-creating-and-cloning-your-repo-4.png)

Click the green "Add People" button and search for my username "pleasework-sh"

![text](image/6-creating-and-cloning-your-repo-5.png)

# Cloning your repository
Go back to your repository homepage.

Click the green "Code" button and copy the URL under SSH.

![text](image/6-creating-and-cloning-your-repo-6.png)

Open your VM and run:

```
cd ~
git clone <your SSH URL here>
```

Change directories into your newly cloned repository. 

