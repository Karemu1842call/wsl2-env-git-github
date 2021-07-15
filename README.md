# Configuring Git, GitHub, and the Flatiron Student Portal on WSL2

## Create a GitHub Account

To work on and get credit for the labs and lessons that you work on during the
program, you will need to sign up for a GitHub account _if you don’t already
have one_.

### Action Item

1. Open the [GitHub signup webpage][] at https://github.com/join
2. Fill out the form and create your account
3. Verify the email address connected to your GitHub account

[GitHub signup webpage]: https://github.com/join

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/mFZOVj8hago" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you were able to verify your email address, continue below.

## Configure Git and GitHub

Git is the tool that we’ll use to download and upload the work we do in labs and
lessons. To use Git without signing in every time, you can create a Secure Shell
(SSH) key and associate that to your GitHub account. Lastly, you will want to
run a few commands to make sure that when you use Git, you get the proper credit
for your work. This step will ask you to do work both in your browser and your
terminal.

### Action Item

1. Open the "Ubuntu" application using the "Start" menu
2. Type `git config --global color.ui true` and press `<Enter>`
3. Type `git config --global user.name` + `<Space>` + your name and press `<Enter>`
4. Type `git config --global user.email` + `<Space>` + the email address you
   used to sign up to GitHub and press `<Enter>`
5. Type `ssh-keygen` and press `<Enter>`, for each prompt do not type anything,
   just continue to press `<Enter>`
7. Type `cat ~/.ssh/id_rsa.pub | clip.exe` and press `<Enter>`. This will copy your SSH key to your clipboard
8. Open the [GitHub New SSH key form][ssh form] (https://github.com/settings/ssh/new)
   _(Note: you need to be logged in to GitHub to access that link.)_
9. Type "My personal PC" in the "Title" input field
10. Paste what’s on your clipboard from step seven in the "Key" input field
11. Click "Add SSH Key"

[ssh form]: https://github.com/settings/ssh/new

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZosWXqhYD00" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you see your new SSH key beneath the "SSH keys" heading, continue below.

## Connect your GitHub Account to your Flatiron School Portal Account

Flatiron School has some helpful tools for you when working on your labs and
lessons through GitHub. For those tools to work, you will need to connect your
Flatiron School Portal account to your GitHub account.

### Action Item

1. Open the [Flatiron School Student Portal webpage][flatiron portal]
   (https://portal.flatironschool.com) _(Note: you need to be logged in to
   Flatiron School Student Portal.)_
2. Connect your GitHub account to your Flatiron School Portal account

[flatiron portal]: https://portal.flatironschool.com

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/nT0vrNNy1-A" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you go back to the [GitHub Account Management webpage][portal github]
(https://portal.flatironschool.com/account/github) and see a red "Disconnect"
button, continue below.

[portal github]: https://portal.flatironschool.com/account/github

## Configure the learn-co gem on Ubuntu

The learn-co gem is the tool that we’ll be using to test and submit the labs and
lessons that we’re working on. Before you can use it, you will need to connect
your Flatiron School Portal account to the copy of the learn-co gem on your
computer. This step will ask you to do work both in your browser and your
terminal.

### Action Item

1. Open the "Ubuntu" application using the "Start" menu
2. Type `touch ~/.netrc && chmod 0600 ~/.netrc` and press `<Enter>` _(Note: you
   may be asked to enter your password.)_
3. Type `learn whoami` and press `<Enter>` _(Note: don’t type anything here yet.)_
4. Go to your [Public Profile Management webpage][]
   (https://portal.flatironschool.com/account/profile) in your browser _(Note:
   if you’re not logged in, you will need to log in again.)_
_(Note: To reduce the work from step 5 to 8 you can click [Account Management][Flatiron Account Management] then continue to the rest of the steps.)_
5. On the top right-hand corner click on your profile picture (This will open a drop down menu).
6. Click on Base.
7. Again on the top right-hand corner click on the profile picture.
8. Click on Account Management.
9.  Copy the string of characters under the "OAuth token" header
10.  Paste the string of characters into the terminal and press `<Enter>`

[Public Profile Management webpage]: https://portal.flatironschool.com/account/profile

[Flatiron Account Management]: https://base.flatironschool.com/account/manage

### Check Your Work

If you see a message with your name, username, and email, continue to the next lesson, **Verify and Troubleshoot Your WSL2 Environment Setup**.
