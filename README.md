#How to Ghost

This is the theme used for http://howtoghost.com

###How to use
	git clone https://github.com/HowtoGhost/howtoghost.git	
	cd howtoghost
	git submodule init
	git submodule update
	mkdir partials
	cp global-resources/partials/* partials/.
	sass assets/sass/screen.scss assets/css/style.css --style compressed
	
###How to Update
	git pull
	git submodule foreach git pull origin master
	chown -R ghost:ghost ./*
	chmod g+w ./*
	cp global-resources/partials/* partials/.
	sass assets/sass/screen.scss assets/css/style.css --style compressed

PR's and suggestions welcome :)