---
layout: post_page
title: Jekyll Adventures
---
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque ultrices ligula quis est maximus facilisis. Nunc et metus vitae nisl pellentesque egestas ac eget orci. Vivamus vel sodales felis. Vestibulum vestibulum bibendum euismod. Nam pellentesque ornare ipsum, quis pharetra eros. Vivamus fringilla id purus non gravida. Maecenas ultrices in ex sed dapibus. Nullam accumsan sit amet enim quis fringilla. Pellentesque dignissim sem ac tristique feugiat. Suspendisse faucibus dui sollicitudin suscipit vehicula. Aliquam dui eros, ullamcorper quis diam non, imperdiet egestas nisl.

Jekyll

Vanilla Bean Creme Theme: http://richbray.me/frap/

Windows 10 x64 Jekyll Install:

Open Powershell v3.

Stop Execution Policy for the session:

	PowerShell.exe -ExecutionPolicy Undefined

Install Chocolatey:

	iwr https://chocolatey.org/install.ps1 -UseBasicParsing | iex

Install Ruby:

	choco install ruby -y
	
Install Development Kit from http://rubyinstaller.org/downloads/.

Initiate Development Kit:

	ruby dk.rb init
	
Open the newly generated config.yml file and append at the end the installation directory with an hyphen and a space first.

Review that the directory is correct and install the dev kit:

	ruby dk.rb review
	ruby dk.rb install
	
Install Jekyll and Bundler:
	
	gem install jekyll bundler
	
Install Jekyll Plugins (Optional):
	
	gem install jekyll-paginate-v2
	gem install jekyll-feed
	gem install jekyll-gist
	gem install rouge
	gem install wdm
	
Install Github-Pages Plugin Dependencies:

	cinst -Source "https://go.microsoft.com/fwlink/?LinkID=230477" libxml2
	cinst -Source "https://go.microsoft.com/fwlink/?LinkID=230477" libxslt
	cinst -Source "https://go.microsoft.com/fwlink/?LinkID=230477" libiconv

Install Nokogiri:
	
	gem install nokogiri
	
Go to an empty directory to create the site and:
	
	jekyll new blogname
	*Enter blogname directory*
	bundle exec jekyll serve
	
All done! Link this folder with your repository and start configuring Jekyll.

Talkling about configuration... I had a hard time changing the theme with Github settings, so if you want to change the theme you should probably do a local test site first, and even then you may need to bundle, build, change the config and gemfile etc. If you want to fiddle with that more info here:
https://jekyllrb.com/docs/themes/

On the other side since Github fully supports Jekyll you could just (probably) copy and paste a theme and adapt it to your needs without building the site per se.

Regular Themes can be found here:
http://jekyllthemes.org/

Gem Packed Themes can be found here:
https://rubygems.org/search?utf8=✓&query=jekyll-theme
