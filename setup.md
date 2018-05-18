# Git installation

In order to use Git, you need to make sure it's available on your platform. Follow the instructions below to make sure you're set up.

## Mac

Luckily, Git comes with Mac by default, but you might need to enable it.

1. Open your terminal. If you've never done this before you can find it in Applications > Utilities > Terminal.
2. Type `git --version` and press enter.
3. If you see something like `git version 2.14.3 (Apple Git-98)` then you're already set up!
4. If you see a popup like the following, then click **Install** and follow the instructions.

	![](http://cdn.osxdaily.com/wp-content/uploads/2014/02/confirm-install-command-line-tools-mac-os-x.jpg)

5. Once installed, go back to step 1 and check you're set up.

## Windows

The easiest way to use Git on Windows is using.... Git for windows.

1. Go to [gitforwindows.org](https://gitforwindows.org/)
2. Click **Download**
3. Click on **Git-2.17.0-64-bit.exe** if you're using a 64-bit version of Windows (most modern versions of Windows are 64-bit). Otherwise click **Git-2.17.0-32-bit.exe**. If you are unsure, there's a [handy guide here](https://support.microsoft.com/en-gb/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64).
4. When you've successfully started the installer, you should see the *Git Setup wizard* screen. 
5. Follow the **Next** and **Finish** prompts to complete the installation. The default options are pretty sensible for most users, so don't worry if you're not sure.

To use it, simply open **Git BASH**. A simple way to do this is to right click the folder you want to work within in Windows Explorer and select **Git BASH**.

![](https://gitforwindows.org/img/gw1.png)

## Linux

Simply install Git with the package manager which comes with your Linux distribution (Ubuntu, Fedora etc).

### Debian (Ubuntu)

1. Open **Terminal**
2. Type `sudo apt-get update` and press enter. You'll be asked for your password. Note that it won't look like you're typing.
3. Type `sudo apt-get install git`

### Fedora

1. Open **Terminal**
2. Type `sudo yum install git` and press enter. You'll be asked for your password. Note that it won't look like you're typing

## Bonus exercise

To start using Git to version control your files, you'll need to provide your name and email address. 

We'll cover this in the workshop, but if you're feeling studious and want to be ahead of the game, then open Terminal (Mac) or Git BASH (Windows):

1. Type `git config --global user.name "Your name"` to set your name.
2. Type `git config --global user.email "your@email.com"` to set your email.

## Helpful links

If you're having trouble, there's a useful guide available at [www.atlassian.com/git/tutorials/install-git](https://www.atlassian.com/git/tutorials/install-git) which covers installing git in some depth. If you're still having trouble, then bring your questions to a Codebar session or the workshop and we'll help you out.
