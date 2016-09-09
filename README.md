#						FFMPEG transition tool


##  What is it?
##  -----------
Script take two video files and, use ffmpeg tool, concatenate they with transition effect.
Now realised three effects: _fade_, _crossfade_, _overlay_.



##  The Latest Version

	version 1.0 2016.09.09
	
##  Whats new

	

##  Installation
You need installed ffmpeg ( http://ffmpeg.org/ ).
Transition tool can be started anywhere.

		
##  Running
Start the script:
```
$ ./fftransition.pl 
Concat two video file with transition effects:
fade (default), crossfade, overlay
Usage: /opt/screen-video1/tools/fftransition.pl --v1=video1.mp4 --v2=video2.avi --out=video_outfile.mp4 [ --effect={fade|crossfade|overlay} ] [ --duration=duration ] [--show] [--help]
where:
	effect - used effect( fade default )
	duration - the time of effect in secounds ( 1 sec default )
	show - show only prepared command, do not execute
Sample:
/opt/screen-video1/tools/fftransition.pl --v1=1.mp4 --v2=2.avi --out=3.mp4 --effect=overlay --duration=3.25

```
If you use _fade_ effect the length of outfile file will be sum of lengths video1 and video2 files. In case _overlay_ and _crossfade_ the 
length of output file will be shorter ( length( video1 )+length( video2 )-2*duration ).


If you wiil only show command (do not make outfile), use key ```--show``` like
```/opt/screen-video1/tools/fftransition.pl --v1=1.mp4 --v2=2.avi --out=3.mp4 --effect=overlay --duration=3.25 --show```


## Known bugs

 
  Licensing
  ---------
	GNU

  Contacts
  --------

     o korolev-ia [at] yandex.ru
     o http://www.unixpin.com

	 