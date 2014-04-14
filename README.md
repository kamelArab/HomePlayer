HomePlayer
==========

How install home player for Freebox HD5


Execute homeplayer.sh

make
killAll vlc

Continue installation and change vlc commande ligne in preference/vlc :

Change :
--intf=${intf} --http-src="${httpSrcDir}" --http-host=127.0.0.1:${httpPort} --sout="#std" --freetype-font="${font}" --config="${vlcrc}" --rtp-client-port=${rtpClientPort}

to

--intf=${intf} --http-src="${httpSrcDir}" --http-host=127.0.0.1 --http-port=${httpPort} --sout="#std" --freetype-font="${font}" --config="${vlcrc}" --rtp-client-port=${rtpClientPort}

Close homeplayer and reexecute homeplayer.sh
