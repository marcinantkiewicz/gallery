# Gallery
The gallery was made as a quick joke to see how much of the first episode of The Great I can fit on a floppy disk (9216 bits). 


Since a video will not fit, and one average frame (png) is already about 400k, I told ffmpeg to sample about 100 frames (ffmpeg -i file.mp4 -r 0.03 out-%03d.png) than turned them into ascii art (for file in  *.png; do img2txt -W 160 -f html $file > ${file%%.png}.html; done). 

The code pulls asciiart html form hard coded url and fills the screen. Left/Right arrows will scroll. This is useless, but  might be a good starting point for something interesting. 
