Simple Readme!

The Emoncms files are pywws services files to provide a link to emoncom.  As they stand they push the external temperature and humidity.

The pywws-livelog file is for your init.d folder.  It will start a livelog process as a daemon on startup (if you have run update-rc.d pywws-livelog defaults).  This was developed from https://gist.github.com/scp93ch/5908666. http://blog.scphillips.com/2013/07/getting-a-python-script-to-run-in-the-background-as-a-service-on-boot/

To monitor the daemon I am using monit (apt get install monit).  As it stands this also monitors the logging process by checking the timestamp on a particular folder.  This file simply goes in the conf.d folder.  Restart monit.

In all cass you will need to adjust these files for locations/names and of course you are responsible afor anythingyou add to your system.

I will try and expand this help at some point.

Cheers
