# Welcome To Whiteboard!

Welcome! Before we begin your first day of camp make sure you've completed the following things.

Pre-requisites 
Make sure you've done the below!

- Code Academy Javascript Track, [click here](https://www.codecademy.com/learn/introduction-to-javascript) to start! (ps. don't worry you won't need to pay)
- Ubuntu Setup (below)


# Ubuntu Setup

Before you start your first day as a developer, we'll need some tools to start developing.

- Github & Git
- Terminal
- A text editor (Visual Studio CODE) - where the bulk of your challenges will be done
- Installing Javascript and NodeJS

## 1. Create your github account

If you haven't already created your github account you can do so below :point_down:

[Sign up to git](https://github.com/join)

Remember to also include a photo of yourself!

## 2. Node.js Setup

bash
sudo apt update
$ sudo apt-get install nodejs

## 3. npm Setup

bash
sudo apt install npm



## 4. Visual Studio Code - Your text editor

Go to https://code.visualstudio.com/Download# and download the .deb file. 


cd Downloads/
sudo apt install ./<file>.deb


## 5. Oh-my-zsh - Pimping your terminal

We will use the shell named `zsh` instead of `bash`, the default one.

bash
sudo apt install zsh


## 6. GitHub

We need to generate SSH keys which are going to be used by GitHub and Heroku
to authenticate you. Think of it as a way to log in, but different from the
well known username/password couple. If you already generated keys
that you already use with other services, you can skip this step.

Open a terminal and type this, replacing the email with *yours* (the
same one you used to create your GitHub account). It will prompt
for information. Just press enter until it asks for a *passphrase*.

bash
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"


This creates a new ssh key, using the provided email as a label.


> Generating public/private rsa key pair.


When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.

> Enter a file in which to save the key (/home/you/.ssh/id_rsa): [Press enter]


At the prompt, type a secure passphrase. 


> Enter passphrase (empty for no passphrase): [Type a passphrase]
> Enter same passphrase again: [Type passphrase again]


Start the ssh-agent in the background.

bash
$ eval "$(ssh-agent -s)"
> Agent pid 59566


Add your SSH private key to the ssh-agent.
bash
$ ssh-add ~/.ssh/id_rsa


[Add the SSH key to your GitHub account.](https://help.github.com/en/articles/adding-a-new-ssh-key-to-your-github-account)


## 7. Postgresql

Later down the weeks we'll talk about SQL and Databases the one we'll be concentrating on his Postgresql,
an open-source robust and production-ready database. 

bash
sudo apt-get install wget ca-certificates
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" >> /etc/apt/sources.list.d/pgdg.list'
sudo apt-get update
sudo apt-get install postgresql postgresql-contrib


Once you've done that, let's check if it worked:

bash
sudo su - postgres
psql


bash
postgres-# \conninfo

To disconnect from PostgreSQL database command prompt just type below command and press enter. It will return you back to the Ubuntu command prompt.

bash
postgres-# \q

# Postman
Postman is used to call http request. This would be useful for testing API later on in the course. [Download here](https://www.getpostman.com/downloads/).

## 8. Last part! Install Visual studio code plugins.

Go to your visual studio code application and open up your extensions.(shift + windows button + x)

1. Search `material theme` and hit install
2. Search `vetur` and also install
3. Reload your visual studio code editor and you should see the changes

