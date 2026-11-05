This is just a simple flow I use for basic bitrate adjustment and conversion. It sets the bitrate to one of your choosing for several different resolutions and resizes anything larger than 1080p to 1080p because that's all I need. It also converts all non-HEVC files to HEVC regardless of bitrate.

To make this work properly, you need to define the bitrates you want in library variables. These are:

bitrate_480p  
bitrate_576p  
bitrate_720p  
bitrate_1080p

I have them set up like this right now:

bitrate_480p    800  
bitrate_576p    900  
bitrate_720p    1200  
bitrate_1080p   1800

In addition to this, you must also install MKVPropEdit for this flow to work. In Linux, it's often a package called mkvtoolnix. In Arch, the package is named mkvtoolnix-cli. I use this tool in this flow to correct any issues in the metadata that could lead to Tdarr incorrectly detecting bitrate specifically in MKV files. 

I might do some audio tuning as well but I'm not sure I need it. This flow was specifically made for my needs. If it helps you, that's great!
