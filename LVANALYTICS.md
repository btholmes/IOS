# Set Up 

    - Permissions problems 
        777 or 644 are fine


    - Set up Composer 
        curl -sS https://getcomposer.org/installer | php
        mv composer.phar /usr/local/bin/composer
        composer update 
    

    - GOOD XAMPP DOWNLOAD 
        https://sourceforge.net/projects/xampp/?source=typ_redirect

	- CPANEL 
		performancebeef.com:2083
		
	- MySQL database
	
	
	
	
	- GitLab
		https://gitlab.com/leyang/PBAnalytics.git
		
		
	- Slack 
		cattlekrush.slack.com
		
	- Toggl
		-toggl.com
	
## Manually Start and Use Serer 

 * Manually start MySQL server for XAMPP 
    sudo /Applications/XAMPP/xamppfiles/bin/mysql.server start
 * Stop use 
    sudo killall mysqld
	
## SHow differences in branches 
    git diff [branchname] origin/master
	
# Mobile Application 
	- PHP Scripts for Database connecdtion
	
	For Development Site []("http://dev.performancebeefanalytics.com/")
	pbanalytics		
	Performance1!
	
	
	
	[](https://performancebeef.com/ (Development)) 
	pbanalaytics
	Performance1
	
	GoDaddy port 2083
	
## Emails 

	-carsonnoble@cattlekrush.com
	
	
## Current Work 
	- Adding a current food available option on Feeds tabs
    - Use the sheets tab to calculate food remaining 

## SQL changes
 * Added total_weight column to feed table 

# Notes 
 * Navigational js is in home/index.php
 * viewdata(post_data, selection) changes views after clicking tab
 * Actual order of function calls from a tab click is 
    update_navigate_icons(val, post_data)
    setActive(val);
    viewdata(post_data, val);

# Problems in Environment 
 * Glyphicons aren't showing 
    Solution: 
    go to http://getbootstrap.com/
    download full bootstrap fill 
    extract four font files into font folder
    restart IDE
 '
# Questions
 * what is feedtype class? Where is it? 

 * All about the feed 
    http://extensionpublications.unl.edu/assets/html/g2093/build/g2093.htm

## Revert Previous Git Pushes

    git checkout [branch] && git reset --hard [commit_id] && git push origin +[branch]


## GAMEPLAN ASSIGNNMENT 1

 * Select pens based on user_id, and the num_heads being > 0 (Carson said < 0 is a testing thing) 

## MySQL Changes 

    ALTER TABLE `feed` ADD `date_added` DATETIME NOT NULL 
    DEFAULT '0000-00-00 00:00:00' AFTER `total_weight`;

## ASK Carson
 
 * edit_feed_db.php error with trying to update feed with current timestamp. 

