---
layout: post

#event information
title:  "Git Install"
cover: "img/FreeAgent_Eva-20.JPG"
date:   2015-03-20
start_time: "10:00"

#event organiser details
organiser: "Lucas Gatsas"


---

<h2 class="section-heading"><strong>Git CommandLines</strong> </h2>







[Git](http://git-scm.com/) is a free software for distributed version control of files that were originally developed for source control of the Linux kernel.



(1.) Go Download Git [Git](http://git-scm.com/download/mac) I'm also a Mac/Unix & Linux User. But this install and Workflow is for Mac Os X. Do you can Download it directly from [sourceforge.net](http://sourceforge.net/projects/git-osx-installer/files/git-2.2.1-intel-universal-mavericks.dmg/download?use_mirror=autoselect). 

(2.)
Open the pkg File with Doppleclick : 


<a href="{{ site.baseurl }}/img/git-sourceforge.png">
    <img src="{{ site.baseurl }}/img/git-sourceforge.png" alt="Lucas Gatsas lucas gatsas" title="lucas gatsas Lucas Gatsas" style="width:100%">
</a>


(3.)
Open Terminal : then type : which git 

(4.)
Type : git  --version

(5.)
Type: git config -l

(6.)
Type: git config --global user.name "[yourusername]"

(7.)
Type: git config --global user.email "[youruseremail@mail.io]"

(8.)
Type: git config -l 

(9.)
Then do you will see your user & email which one do you have set up right now!

exmaple 

<code> user.name=[yourusernamewillshowuphere]</code>

<code>user.email=[youruseremailwillshowuphere]</code>


Have fun with Git! 
Below do you will see some Git CommandLines 

<br> 



<div class="alert alert-info">
<strong>Git Terminology:</strong><br>
<table class="table table-responsive">
<tbody>
<tr>
<td>
master
</td>
<td>
default branch we develop in
</td>
</tr>
<tr>
<td>
origin
</td>
<td>
default upstream repo (Github)
</td>
</tr>
<tr>
<td>
HEAD
</td>
<td>
current branch
</td>
</tr>
<tr>
<td>
remote
</td>
<td>
repository stored on another computer
</td>
</tr>
<tr>
<td>
staging (adding)
</td>
<td>
adding changed files to index tree to be committed
</td>
</tr>
</tbody>
</table>
<p>
Here’s a good <a href="http://stackoverflow.com/questions/7076164/terminology-used-by-git" target="_blank" class="alert-link">glossary</a> of definitions.
</p>
</div>



<br>


<h2 class="section-heading"><a href="#starting-a-repo-init/clone/remote"><span class="heading-link ti-link"></span> Starting a Repo <small>init/clone/remote</small></a></h2>









<table class="table table-responsive table-hover">
<tbody>
<tr>
<td>

	<code>
	git init
	</code>

</td>
<td>
Create a repo from existing data
</td>
</tr>
<tr>
<td>

	<code>
git clone (repo_url)
</code>

</td>
<td>
Clone a current repo (into a folder with same name as repo)
</td>
</tr>
<tr>
<td>

	<code>
git clone (repo_url) (folder_name)
</code>

</td>
<td>
Clone a repo into a specific folder name
</td>
</tr>
<tr>
<td>

	<code>
git clone (repo_url) .
</code>

</td>
<td>

Clone a repo into current directory (should be an empty directory)

</td>
</tr>
<tr>
<td>

<code>
git remote add origin 
	https://github.com/
	username/
	(repo_name).git
</code>

</td>
<td>
Create a remote repo named origin pointing at your Github repo (after you’ve already created the repo on Github) (used if you git init since the repo you created locally isn’t linked to a remote repo yet)
</td>
</tr>
<tr>
<td>

<code>
git remote add 
	origin git@github.com:
	username/
	(repo_name).git
</code>

</td>
<td>
Create a remote repo named origin pointing at your Github repo (using SSH url instead of HTTP url)
</td>
</tr>
<tr>
<td>

	<code>
git remote
</code>

</td>
<td>
Show the names of the remote repositories you’ve set up
</td>
</tr>
<tr>
<td>
	<code>

git remote -v
</code>

</td>
<td>
Show the names and URLs of the remote repositories
</td>
</tr>
<tr>
<td>
	<code>

git remote rm 
	(remote_name)
	</code>

</td>
<td>
Remove a remote repository
</td>
</tr>
<tr>
<td>

<code>

git remote set-url 
	origin (git_url)
	</code>

</td>
<td>
Change the URL of the git repo
</td>
</tr>
<tr>
<td>

	<code>

git push
</code>

</td>
<td>
Push your changes to the origin
</td>
</tr>
</tbody>
</table>


<br>



<h2 class="section-heading"><a href="#showing-changes-status/diff/log/blame"><span class="heading-link ti-link"></span> Showing Changes <small>status/diff/log/blame</small></a></h2>







<table class="table table-responsive table-hover">
<tbody>
<tr>
<td>
	<code>
git status
</code>
</td>


<td>
Show the files changed
</td>
</tr>
<tr>
<td>

	<code>
git diff
</code>
</td>



<td>
Show changes to files compared to last commit
</td>
</tr>
<tr>
<td>

	<code>
git diff (filename)
</code>
</td>


<td>
Show changes in single file compared to last commit
</td>
</tr>
<tr>
<td>

	<code>
git diff (commit_id)
</code>
</td>


<td>
Show changes between two different commits.
</td>
</tr>
<tr>
<td>
	<code>
git log
</code>
</td>


<td>
Show history of changes
</td>
</tr>
<tr>
<td>
	<code>
git blame (filename)
</code>
</td>
<td>
Show who changed each line of a file and when
</td>
</tr>
</tbody>
</table>


<br>



<div class="alert alert-info">
<strong>Commit ID:</strong> This can be that giant long SHA-1 hash. You can call it many different ways. I usually just use the <strong>first 4 characters</strong> of the hash.
</div>


<br>




<h2 class="section-heading"><a href="#undoing-changes-reset/revert"><span class="heading-link ti-link"></span> Undoing Changes <small>reset/revert</small></a></h2>





<table class="table table-responsive table-hover">
<tbody>
<tr>
<td>
	<code>
git reset –hard
</code>
</td>
<td>
Go back to the last commit (will not delete new unstaged files)
</td>
</tr>
<tr>
<td>
	<code>
git revert HEAD
</code>
</td>
<td>
Undo/revert last commit AND create a new commit
</td>
</tr>
<tr>
<td>
	<code>
git revert (commit_id)
</code>
</td>
<td>
Undo/revert a specific commit AND create a new commit
</td>
</tr>
</tbody>
</table>




<br>



<h2 class="section-heading"><a href="#staging-files-add/rm"><span class="heading-link ti-link"></span> Staging Files <small>add/rm</small></a></h2>






<table class="table table-responsive table-hover">
<tbody>
<tr>
<td><code>
git add -A</code>
</td>
<td>
Stage all files (new, modified, and deleted)
</td>
</tr>
<tr>
<td><code>
git add .</code>
</td>
<td>
Stage new and modified files (not deleted)
</td>
</tr>
<tr>
<td><code>
git add -u</code>
</td>
<td>
Stage modified and deleted files (not new)
</td>
</tr>
<tr>
<td><code>
git rm (filename)</code>
</td>
<td>
Remove a file and untrack it
</td>
</tr>
<tr>
<td><code>
git rm (filename) –cached</code>
</td>
<td>
Untrack a file only. It will still exist. Usually you will add this file to .gitignore after rm
</td>
</tr>
</tbody>
</table>


<br>


<div class="alert alert-info">
<strong>Git Workflow Trees:</strong> How adding and committing moves files between the different git trees.
</div>
<br>



<table class="table table-responsive">
<tbody>
<tr>
<td>
Working Tree
</td>
<td>
The “tree” that holds all our current files.
</td>
</tr>
<tr>
<td>
Index (after adding/staging file)
</td>
<td>
The “staging” area that holds files that need to be committed.
</td>
</tr>
<tr>
<td>
HEAD
</td>
<td>
Tree that represents the last commit.
</td>
</tr>
</tbody>
</table>



<br>

<h2 class="section-heading"><a href="#publishing-commit/stash/push"><span class="heading-link ti-link"></span> Publishing <small>commit/stash/push</small></a></h2>





<table class="table table-responsive table-hover">
<tbody>
<tr>
<td><code>
git commit -m “message”</code>
</td>
<td>
Commit the local changes that were staged
</td>
</tr>
<tr>
<td><code>
git commit -am “message”</code>
</td>
<td>
Stage files (modified and deleted, not new) and commit
</td>
</tr>
<tr>
<td><code>
git stash</code>
</td>
<td>
Take the uncommitted work (modified tracked files and staged changes) and saves it
</td>
</tr>
<tr>
<td><code>
git stash list</code>
</td>
<td>
Show list of stashes
</td>
</tr>
<tr>
<td><code>
git stash apply</code>
</td>
<td>
Reapply the latest stashed contents
</td>
</tr>
<tr>
<td><code>
git stash apply (stash_id)</code>
</td>
<td>
Reapply a specific stash. (stash id = <strong>stash@{2})</strong>
</td>
</tr>
<tr>
<td><code>
git stash drop (stash_id)</code>
</td>
<td>
Drop a specific stash
</td>
</tr>
<tr>
<td><code>
git push</code>
</td>
<td>
Push your changes to the origin
</td>
</tr>
<tr>
<td><code>
git push origin (local_branch_name)</code>
</td>
<td>
Push a branch to the origin
</td>
</tr>
<tr>
<td><code>
git tag (tag_name)</code>
</td>
<td>
Tag a version (ie v1.0). Useful for Github releases.
</td>
</tr>
</tbody>
</table>

<br>


<h2 class="section-heading"><a href="#updating-and-getting-code-fetch/pull"><span class="heading-link ti-link"></span> Updating and Getting Code <small>fetch/pull</small></a></h2>






<table class="table table-responsive table-hover">
<tbody>
<tr>
<td><code>
git fetch</code>
</td>
<td>
Get the latest changes from origin (don’t merge)
</td>
</tr>
<tr>
<td><code>
git pull</code>
</td>
<td>
Get the latest changes from origin AND merge
</td>
</tr>
<tr>
<td><code>
git checkout -b (new_branch_name) origin/(branch_name)</code>
</td>
<td>
Get a remote branch from origin into a local branch (naming the branch and switching to it)
</td>
</tr>
</tbody>
</table>

<br>

<h2 class="section-heading"><a href="#branching-branch/checkout"><span class="heading-link ti-link"></span> Branching <small>branch/checkout</small><br>
</a></h2>







<table class="table table-responsive table-hover">
<tbody>
<tr>
<td><code>
git branch</code>
</td>
<td>
Show all branches (local)
</td>
</tr>
<tr>
<td><code>
git branch -a</code>
</td>
<td>
Show all branches (local and remote)
</td>
</tr>
<tr>
<td><code>
git branch (branch_name)</code>
</td>
<td>
Create a branch from HEAD
</td>
</tr>
<tr>
<td><code>
git checkout -b (branch_name)</code>
</td>
<td>
Create a new branch and switch to it
</td>
</tr>
<tr>
<td><code>
git checkout (branch_name)</code>
</td>
<td>
Switch to an already created branch
</td>
</tr>
<tr>
<td><code>
git push origin (branch_name)</code>
</td>
<td>
Push a branch up to the origin (Github)
</td>
</tr>
<tr>
<td><code>
git checkout -b (new_branch_name) origin/(branch_name)</code></td>
<td>
Get a remote branch from origin into a local branch (naming the branch and switching to it)
</td>
</tr>
<tr>
<td><code>
git push origin –delete (branch_name)</code>
</td>
<td>
Delete a branch locally and remotely
</td>
</tr>
</tbody>
</table>

<br>


<h2 class="section-heading"><a href="#integrating-branches-merge/rebase"><span class="heading-link ti-link"></span> Integrating Branches <small>merge/rebase</small><br>
</a></h2>




<table class="table table-responsive table-hover">
<tbody>
<tr>
<td>
<code>git checkout master </code> <br> <code>git merge (branch_name)</code>
</td>
<td>
Merge a specific branch into the master branch.
</td>
</tr>
<tr>
<td>
<code>git rebase (branch_name)</code>
</td>
<td>
Take all the changes in one branch and replay them on another. Usually used in a feature branch. Rebase the master to the feature branch so you are testing your feature on the latest main code base. Then merge to the master.
</td>
</tr>
<tr>
<td>
<code>git cherry-pick (commit_id)</code>
</td>
<td>
Merge just <strong>one specific commit</strong> from another branch to your current branch.
</td>
</tr>
</tbody>
</table>

<br>



<div class="alert alert-info">
<strong>Merging:</strong> Merging will occur <strong>FROM</strong> the branch you name <strong>TO</strong> the branch you are <em>currently</em> in. <strong>Rebasing:</strong> Usually switch to a feature branch (<code>git checkout newFeature</code>). Then rebase (<code>git rebase master</code>). Then merge back so you have all the changes of master and the feature branch (<code>git checkout master</code>, and <code>git merge newFeature</code>).
</div>

<br>





<small>Image : Building Of The Trojan Horse Giovanni Domenico Tiepolo</small>


<blockquote>
	"Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency."
</blockquote>