git config --global user.name <username>	(Change git user name)
git config --global user.email <useremail>	(Change git user email)

git status 			(Show the status of the actual staging zone)
git add . 			(Add every file of the current dir to the stage)
git add <filename>		(Add the specified file to the stage)
git rm --cached <filename>	(Remove the file from the stage)
git commit -m "<description>"	(Commit all the staging zone)
git log				(Show all the differents commits done yet)
git log --oneline		(Show the differents commits in one line each)

git checkout <commitID>		(See the state of the code at one commit)
git checkout <branchname>	(Go to the head of the branch)

git revert <commitID>		(Make a new commit that revert the commit with this ID ":wq")

git reset <commitID>    (Erase all the commits before the one with this ID but no change in editor)
git reste <commitID> --hard	(Same but also change in editor)

git branch <branchname>		(Create a new branch give it a name)
git branch -a			(Show all the branches)
git checkout <branchname>	(Change branch)
git branch -D <branchname>	(Delete the named branch if not merged)
git branch -d <branchname>	(Delete the named branch if merged)
git checkout -b <banchname>	(Create a new branch and goes on it)

git merge <branchname>		(Merge the named branch in the actual branch)
TIPS : For conflict, fix it and commit the result


git push <url/alias> <branchname> 	(Push the named branch in the online repositry selected)
git remote add <alias> <url> 		(Give to the online repo an alias for the local repo)
git remote -v 				(Show all the alias for this repo repoalias is "origin" if cloned from github)
git clone <url>				(Clone the url's repo in the actual directory)
git pull <url/alias> <branchname>	(Merge the branch from the url to the local branch)

TIPS : Always better to push side branches and then create pull request on GitHub (you can pull several pushs in one merge)
Forking is cool
