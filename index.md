# Git - the #1 source code control tools

## Training Agenda

* Introduction Git
* Version Control History, GIT Design Goal
* GIT Extension Installation and Setup
* GIT Concept and Terminology
* GIT Daily Usage in SVN way
* Create your own GIT repo (local & remote)
* New GIT feature and further more manual

> press `m` to see overview slide;
> press `g` to goto slide by number.
> <cite>Training material prepared by Eric Guo</cite>

## Git and Github from CNY Ticket

<iframe src="http://it.21cn.com/mi/a/2013/0123/08/20262835.shtml" width="1024" height="768" frameborder="0"></iframe>

## Github and non-programming usage

* [Chicago pedway/bike-routes/building-foorprints](https://github.com/Chicago)
* [German Federal Laws](https://github.com/bundestag/gesetze#german-federal-laws-and-regulations)
* [New Zealand Act Record](https://github.com/Br3nda/legislation/tree/master/act/public)

## Version Control History

* Manually keep track of versions of code! (1960s)
* Keep lots of versions in one file! (1972, SCCS)
* You can each have your own copy checked out! (1982, RCS)
* Version multiple files at once! (1986, CVS, atomic by Subversion 2000)
* Shared repository can be on a remote machine! (1994, CVS with )
* Open source version control hosting! (1999, SourceForge)
* No central repository! (2005, GIT)
* When you checkout that’s a fork too, and you can do that in public! (2008, GIThub)

[source](http://www.flourish.org/blog/?p=397)

## GIT & GitHub History

Torvalds wanted a distributed system that he could use like BitKeeper, but none of the available free systems met his needs, particularly his performance needs. From an email he wrote on 7 April 2005 while writing the first prototype.

GitHub is a web-based hosting service for software development projects that use the Git revision control system. GitHub offers both commercial plans and free accounts for open source projects. According to the Git User's Survey in 2009, GitHub is the most popular Git hosting site.

## GIT Design Goal

* Take CVS as an example of what not to do; if in doubt, make the exact opposite decision.

* Support a distributed, BitKeeper-like workflow

* Very high performanc and strong safeguards against corruption, either accidental or malicious


## GIT Extension Design Goal

* GitExtensions is a shell extension, a Visual Studio 2008 / 2010 plug-in and a standalone GIT repository tool.

* Great tools enable you think and work in Unix style gradually

## GIT Extension Install - All User

[http://code.google.com/p/gitextensions/](http://code.google.com/p/gitextensions/) (download URL)

![Installation Step 1](git-training/installation_step_01.png "Install for all users")

## GIT Extension Install - Both

![Installation Step 2](git-training/installation_step_02.png "Both need")

## GIT Extension Install - Integration

![Installation Step 3](git-training/installation_step_03.png "Not need items")

## GIT Extension Install - PuTTY

![Installation Step 4](git-training/installation_step_04.png "Using PuTTY")

## GIT Extension Install - KDiff3

![Installation Step 5](git-training/installation_step_05.png "Even documentation also can not select")

## GIT Extension Install - MsysGIT

![Installation Step 6](git-training/installation_step_06.png "No need context menu need")

## GIT Extension Install - Bash Only

![Installation Step 7](git-training/installation_step_07.png "Bash only")

## GIT Extension Install - cross-platform

![Installation Step 8](git-training/installation_step_08.png "cross-platform")

## GIT Extension Setup

GIT Extension -> Settings -> Settings to fill:

    * User Name
    * eMail

![Setup 01](git-training/setup_username_email.png "Username and email")

## GIT Generate SSH Key

GIT Extension -> Remotes -> PuTTY -> Generate or import key:

![Setup 02](git-training/setup_generate_sshkey.png "Generate SSH Key")

## GIT Email your Public key to Admin

1. Copy selection text and email to your Admin
2. Save private key because you need private key to login latter
3. Loss private key need regenerate private key and resent public key to Admin

![Setup 03](git-training/setup_email_public_key.png "email public key")

## GIT clone your first repositories

Repository to clone: *gitolite@cvpscmip01:testing.git*

![Test 01](git-training/test_clone_first_repository.png "Clone the first repository")

## GIT Commit/Push your first change

![Test 02](git-training/test_commit_first_change.png "Commit your first change")

## GIT Daily Usage in SVN way

* Clone (SVN Checkout)
* Commit (in Local)
* Push (SVN Commit)
* Pull (SVN Update All)
* gitK (SVN History)

## GIT Concept and Terminology

![Concept and Terminology](git-training/git_concept_and_terminology.png "GIT Concept and Terminology")

## gitk - a GUI commit viewer for git

![a commit viewer for git](git-training/gitk_commit_viewer_screen.png "gitk_commit_viewer")

## GIT Key Sales Point

1. Very fast and user friendly
1. Source Code Repository is distributed, isolated, history complete
1. All action can run in Local except pull and push
1. Submit and rollback always success (until pull and push)
1. Can fix last submit very easily

## Create your GIT repository in GIT Extension

Open Repopsitory -> Your not GIT init yet folder -> Initialize Repository

![create repository](git-training/create_repository_init.png "Create GIT repository")

## Add .gitignore for VS.NET intermediate files

Forgot any add ignore file and pattern in Subversion, now it’s a One-click only action!

![add gitignore](git-training/create_repository_gitignore.png "Add .gitignore")

# Don’t forgot to add ignore files!

## Add .gitignore to ignore VS.NET *intermediate* files

#### The obj/exe or any other binary file will make repository looks like amature job!

![add gitignore](git-training/create_repository_gitignore.png "Add .gitignore")

## Commit initial version of files

![initial commit](git-training/create_repository_initial_commit.png "Initial Commit")

## Push your repository to CVPSCMIP01

You can to put any repository to:  (no need inform GIT admin!)

    gitolite@cvpscmip01:/usr/[*yourname*]/[*your_repository_name*]

![push to server](git-training/create_repository_push_gitolite.png "Push to server")

## Your repository is visible at Web!

1. Work as own at first in your usr folder. (No need to inform GIT Admin)
2. Rise your project to root folder if it is company widely used and relatively stable. (Need GIT Admin help)
3. Old Subversion project will moved to root folder by GIT Admin already

#### [http://cvpscmip01/usr/eric/MTtest-Assistant.git](http://cvpscmip01/usr/eric/MTtest-Assistant.git)

## More GIT tricks need SSH and console now

Setting description for your own repository:

    6749@SHE127731 /c/git
    $ echo "A semi-auto MES Yield Limit Batch setting tools used in SPAS 125-001" | ssh gitolite@cvpscmip01 setdesc usr/eric/YieldLimits-Change
    Enter passphrase for key '/c/Users/6749/.ssh/id_rsa':

New description is: *A semi-auto MES Yield Limit Batch setting tools used in SPAS 125-001* now

## Introduction Gitlab

Access it [at](http://cvpgitip01.sandisk.com/)

## A successful Git branching model

![Git Branch Model](git-training/git_branching_model.png "The typical Git branch model")

[source](http://nvie.com/posts/a-successful-git-branching-model/)

## More document and essay about GIT

* Git Extensions User Manual (in your hard drive after install GIT Extension)
* [Pro GIT](http://progit.org/book/) ([中文](http://progit.org/book/zh/))
* [GIT Magic](http://www-cs-students.stanford.edu/~blynn/gitmagic/) ([中文](http://www-cs-students.stanford.edu/~blynn/gitmagic/intl/zh_cn/))
* [Git Tips集锦](https://gitcafe.com/riku/GitTips)
* [Git权威指南](http://www.worldhello.net/gotgit/)

Things we not mentioned:

    GIT command line
    Branch, Merge, Rebase, Cherry Pick

# Question & Answer ?