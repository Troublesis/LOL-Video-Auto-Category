# LOL-Video-Auto-Category
Python script which will automatically sort League of legends videos base on the game mode and champion which was in the video.

I created a little python script which will automatically sort League of legends videos base on the game mode (currently only support normal / aram) and champion which was in the video. I am a new python learner and the code still has some issues. I am still happy it is partically working. Hope you will find this code is useful and hope you can help me to improve this code. Please let me knwo if you have any good ideas and give some advice on how to improve the code.

Note: While I am playing League of Legends, I always use [Overwolf - GameSummary](https://www.overwolf.com/app/overwolf-game_summary "Overwolf - GameSummary - Bookmark") to automattically record the gameplays. It is a really good free applications. Highly recommended.

The app will automatically save the gameplays video in your local drive with folder name format as - League of Legends_DD-MM-YYYY_HH-mm-ss. Since the folder name does not show which champion I was playing, this is the reason why I create this code to help me to automatically detect which champion I was playing in the recorded videos.

=========================================

# Code Running Sample
![](/GIF/lolVideoDetectCodeRunningSample.gif)

# Info
The code is detecting champion based on the frame.jpg image capture from the detecting video and campare the champion icon in the image with the full champion icons library. If the championIcon image found in the frame then the code will return the champion name. If the championIcon not found. It will return an undefined championIcon.jpg. We will have to mannually add the undefined Champion Icon Image into [Champion Icon Library](https://github.com/Troublesis/LOL-Video-Auto-Category/blob/master/Screenshots/championIconLibrary.jpg "Champion Icon Library Screenshot")

![frame.jpg captured from video frame](/Screenshots/frame.jpg)
frame.jpg<br/><br/>
![championIcon.jpg cropped from frame.jpg](/Screenshots/championIcon.jpg)<br/>
championIcon.jpg

# Run the code
1. Download [lolVideoAutoCategory.zip](https://github.com/Troublesis/LOL-Video-Auto-Category/blob/master/lolVideoAutoCategory.zip "lolVideoAutoCategory")
2. Extract the file<br/>
![File list of lolVideoAutoCategory.zip](/Screenshots/codeFiles.jpg)<br/>
3. Run lolVideoAutoCategory.py<br/>
   Enter root video folder path<br/>
   Enter new video storage folder path<br/>
![Running lolVideoAutoCategory.py](/GIF/runningCode.gif)<br/>

# To Do List
make champion detection function more accurate<br/>
detect all champions in the video<br/>
detect final kda in the video<br/>
detect more game mode (eg. urf/teamfight tactics)<br/>

# Known Issues
* I marked in the comments in the code as 'fix:' 'error:' with some known issues
* error: when the selected video is not accessable the code will be terminated
