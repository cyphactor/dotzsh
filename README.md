# My .zshrc setup

This is my personal **.zsh** directory setup which contains my **.zshrc** and
any dependency scripts that my **.zshrc** uses most likely for its prompts.

## Set shell to /bin/zsh

If you are on a Mac OS X box and want to use this **.zsh** setup you have to
first switch your account to use `/bin/zsh`. This is done by following the
steps presented below.

1. Go to **System Preferences**
2. Select **Users & Groups** under the **System** section
3. Click the Lock icon in the lower left corner to unlock the preferences
4. Enter your password to actually unlock the preferences
5. Right click on your user in the list on the left and select **Advanced
   Options**
6. From the **Login shell:** drop-down select `/bin/zsh`
7. Click the **OK** button
8. Close **System Preferencs**

At this point if you create a new Terminal instance it should open up with
`/bin/zsh` as your shell. You can verify this by running the following command
and verifying that the output is `/bin/zsh`.

    echo $SHELL

Once you have verified you are running `/bin/zsh` as your shell you can
install this **.zsh** setup using the instructions below.

## Installation

To install this **.zsh** setup simply run the following commands.

    cd ~/
    git clone git@github.com:cyphactor/dotzsh.git ~/.zsh
    ln -s ~/.zsh/zshrc .zshrc

## Update

To get the latest version of this setup at any time simply run the following
commands.

    cd ~/.zsh
    git pull --ff-only

Thats it! Assuming you didn't have any local commits that prevent it from
being fast-forwarded when pulled in. If you do happen to have local changes
commited to the **master** branch locally, you should really create a new
topic branch pointing to them and reset --hard your local master back to the
official origins remote master.
