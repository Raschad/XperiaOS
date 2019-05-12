XperiaOS
========

	mkdir xos
	cd xos
	
To initialize your local repository, use this command:

	repo init -u https://github.com/Raschad/XperiaOS.git -b pie
 
 Create local_manifests folder
---------------
    mkdir .repo/local_manifests
    
Download manifest: 

    curl https://raw.githubusercontent.com/raschad/manifest-1/xperia-pie/roomservice.xml > ~/xos/.repo/local_manifests/roomservice.xml    
 
 Then to sync up:


	repo sync -f --force-sync --no-tags --no-clone-bundle -j32

Build:

    . build/envsetup.sh
    lunch
or
    
    brunch honami
