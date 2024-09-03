# Introduction to the Linux and command line tools
When we refer to "Linux" we are referring to a family of **operating systems**. 

For now, just note that Linux operating systems run the majority of the world, that is, the majority of web servers run some sort of Linux-based operating system. Many of these web servers are **headless**, meaning they lack a graphical user interface (GUI). When you hear GUI, think of being able to click around with a mouse. Your personal PC or laptop has a GUI if you can use your mouse. 

Thus, headless servers can only be interacted with using a keyboard, no mouse. The reason many servers are headless is to save computing power. Regardless of whether a system has a GUI, many tools you will run into in your career lack a GUI but do have a command-line option to run them. The command line will quickly become your friend. 

# Linux command line training
Please complete the tutorial over at [terminaltutor.com](https://www.terminaltutor.com/). Then, try out some of these commands in your virtual machine.

# Using Git
To track changes in our code and push our changes to our GitHub repositories, we will be using `git` - a command-line based tool. 

## SSH Key Setup
In order to push code from your local repository into GitHub (the remote repository) - we need to setup our own **SSH key** for authentication. SSH stands for Secure Shell and is a protocol often used for remote access into machines, but we can use it to interface with our GitHub repositories as well. Communications through SSH are encrypted. 


### Steps to setup your SSH key

Log into your VM. 

Run the following command, replacing the placeholder email with your own:
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

When you're prompted to "Enter a file in which to save the key", you can press Enter to accept the default file location. 
```
> Enter a file in which to save the key (/Users/YOU/.ssh/id_ALGORITHM): [Press enter]
```

Then, type a secure passphrase.
```
> Enter passphrase (empty for no passphrase): [Type a passphrase]
> Enter same passphrase again: [Type passphrase again]
```

Then run the following commands, replacing the placeholder values with your own information. 

``` 
git config --global user.name "[name]"
git config --global user.email "[email address]"
```

To grab your public ssh key you can run 
```
cat <insert_name_of_ssh_file>.pub
```
and copy it to your clipboard. If you did not install guest additions in your VM and enabled your bi-directional clipboard  you may want to log into your GitHub account from the web browser of your VM and complete the steps there. If you are having trouble with this, please see me during office hours or in class.

In the upper-right corner of any page on GitHub, click your profile photo, then click Settings.

In the "Access" section of the sidebar, click SSH and GPG keys.

Click New SSH key or Add SSH key.

In the "Title" field, add a descriptive label for the new key. For example, if you're using a personal laptop, you might call this key "Personal laptop".

Select the key type as "Authentication".

In the "Key" field, paste your public key.

Click Add SSH key.

The steps I've included are taken /remixed slightly from the following URLs:
- [Generating a new SSH Key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key)
- [Adding a new SSH Key to your GitHub account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

