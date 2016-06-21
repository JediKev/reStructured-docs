# :computer: reStructured Docs

### Description
A guide to write and push reStructuredText documentation to GitHub using only the Atom text editor. Here you will be using the Git-Plus Atom package, forking and cloning a documentation repo, and adding/committing/pushing some changes to GitHub.

#### 1. Check for Git-Plus Atom package
Open Atom and go to `Atom > Preferences`.  Once here you will see a tab menu on the left.  Look for the tab labeled 'Packages' and click on it.  Here you will see a list of all packages installed on your Atom editor.  You can either scroll and look for the one labeled 'git-plus' or you can search for it with the search bar at the top.  If you see it listed congratulations, you can move to the next step!  If not you can go to my guide on how to [set up your environment](https://github.com/JediKev/reStructured-docs-setup) for this and then go to the next step.

#### 2. Fork documentation repo
In order to take another developers repo and make changes to it without affecting their master code, you first have to fork the repo.  This basically makes a fresh copy of the master code from their repo and puts it in a repo on your account. So on [this repo](https://github.com/JediKev/reStructured-docs) look at the top right of the page and you'll see a button labeled 'Fork', click this button and it will automatically fork the repo to your account.  Now you can navigate to your repositories list and find the forked repo!

#### 3. Clone documentation repo
Go to your profile and click on 'Repositories', find and open the repo you just forked.  On the right hand side you will see a green button labeled 'Clone or Download'.  Click this button and a drop down with a link should appear.  If you have your [SSH key set up](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/) on GitHub then click the clipboard icon on the right to copy the link to your clipboard.  Then open Terminal and `cd` to wherever you want the repo to live.  Once there type:
```
$ git clone git@github.com:repo/link.git
```
Replacing the example link with the repo link you copied.
>If you don't have your SSH key set up, then you need to press the download button and save the repo wherever you want it.

#### 4. Open repo in Atom
Now that you have the repo saved, open Atom and go to `File > Add Project Folder`.  A new window should open with your finder.  Navigate to where you saved the repo, highlight the repo folder and press open.  Atom should pop up with your repo on the left side.

#### 5. Make changes
Once your repo is in Atom you can open it by clicking the arrow next to the name on the sidebar and click the `Example.rst` file.  Once open follow the instructions to make your first reStructuredText file!
