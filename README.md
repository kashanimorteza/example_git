<!---------------------------------------[Description]-->
## Description
    This is a example of git


<!---------------------------------------[Diagram]-->
<br><br>

## Diagram

<div align="left"><img src="git.jpeg"></div>




<!---------------------------------------[Concept]-->
<br><br>

## Concept 

گیت یک مخزن (repository) می سازه که از سه لایه منطقی به فایل ها نگاه میکنه :
<br>
1 – لایه اول یا همان (working tree) که هنوز اقدامی برای ثبت تغییرات انجام نشده و فایل ها در حال تغییر هستند 
<br>
2 – لایه دوم یا همان (stage)که با وارد کردن فایل ها به این لایه، آنها آماده ثبت تغییر می شوند
<br>
3 – لایه سوم (Repository) که تمام تغییرات فایل ها ثبت می شوند




<!---------------------------------------[Source]-->
<br><br>

## Source

#### General
<a href="http://git-scm.com" target="_blank">git-scm</a> - 
<a href="http://github.com" target="_blank">github</a> - 
<a href="http://gitlab.com" target="_blank">gitlab</a>

#### Tutorial
<a href="http://faradars.org" target="_blank">faradars</a> - 
<a href="http://roocket.ir" target="_blank">roocket</a> - 
<a href="http://clicksite.org" target="_blank">clicksite</a> - 
<a href="http://faranesh.com" target="_blank">faranesh</a> -
<a href="https://gitexplorer.com/" target="_blank">gitexplorer</a> 



<!---------------------------------------[Install]-->
<br><br>

## Install

#### Mac
    brew install git

#### Ubuntu
    sudo apt install git-core
    sudo apt install git-all

#### Windows (Someone who uses the Linux will have steps with confidence and authority)
    ...


<!---------------------------------------[Config]-->
<br><br>

## Config

#### User

    git config --global user.email "kashani.morteza@gmail.com"      
    git config --global user.name "morteza"

#### Color highlighting

    git config --global color.ui true
    git config --global color.status auto
    git config --global color.branch auto

#### Setting default editor
    
    git config --global core.editor vim

#### Setting default merge tool

    git config --global merge.tool vimdiff

#### Listing Git settings
    
    git config --list


<!---------------------------------------[Github Add ssh key]-->
<br><br>

## Github Add ssh key

#### linux
    
	git config --global user.email "abdcoin1001@gmail.com"      
	git config --global user.name "abd"
	git config --global core.editor "vim"

	1 - mkdir /home/abd/.ssh
	2 - cd /home/abd/.ssh
	3 - ssh-keygen -t rsa -b 2048 -C "abdcoin1001@gmail.com"
		choose name : gitlab
	4 - cat /home/abd/.ssh/gitlab.pub
	5 - Copy key and add to gitlab ssh key gitlab > User Settings > preferences > SSH Keys
	6 - vim /home/abd/.ssh/config 
		# GitLab.com
		Host gitlab.com
			PreferredAuthentications publickey
			IdentityFile /home/abd/.ssh/gitlab
	7 - ssh -T git@gitlab.com

#### Windows

    1 - run git program
    2 - ssh-keygen -t rsa -b 2048 -C "kashani.morteza@gmail.com"
	3 - Go to C:/Users/Administrator/.ssh/
	4 - Copy id_rsa.pub and add to gitlab ssh key gitlab > User Settings > preferences > SSH Keys




<!---------------------------------------[Tools]-->
<br><br>

## Tools
    Ohmyzsh : graphic for git



<!---------------------------------------[Structure]-->
<br><br>

## Structure

<!-----------[Config]-->
#### Config 
    Level
    -------------------
    Local
    Global
    System
    worktree

    Object
    -------------------
    user
    color highlighting
    default editor
    default merge tool

<!-----------[File track]-->
#### File track
    Work directory
    Stage
    Repository

<!-----------[File Level]-->
#### File level
    Repository
    Branch
    Tag
    Version

<!-----------[Location]-->
#### Location
    Local
    Remote

<!-----------[Command]-->
#### Command
    Start a working area
    Work on the current change
    Examine the history and state 
    grow, mark and tweak your common history
    Collaborate