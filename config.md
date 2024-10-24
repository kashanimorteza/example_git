<!---------------------------------------[Genaral]-->
## General

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

#### Linux
    
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


<!---------------------------------------[Git Ignore]-->
<br><br>

## Git Ignore

	git config --global core.excludesfile ~/.gitignore

	vim .gitignore
	--------------------
	videos/
	sound/1.mp3
	*.dll
	!myfolder/m.dll