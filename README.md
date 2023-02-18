# maplestory-culvert-flag-score-extractor
Extracts guild's IGNs, Culvert, and Flag Race numbers from video of member participation status by using Tesseract OCR and Python 

## STEPS
### 1. TESSERACT OCR
Download https://www.dropbox.com/s/2m97m85bl8wsb18/Tesseract-OCR.zip?dl=0 and unzip into maplestory-culvert-flag-score-extractor folder.

### 2. Recording
Record a scrolling cropped video from top of the list and bottom by scrolling. Make sure the cursor doesn't show up and there are no headers or extra space, like shown below, and save it in culver-flag-parser folder. If the video isn't in HD there is a higher chance mistakes occur in numbers. Works best in 1920x1080. May need to increase resizing if it's in a lower resolution, resulting in longer runtime.

![](https://github.com/j3li/maplestory-culvert-flag-parser/blob/main/recording%20example.gif)

### 3. Running the Code
Create a `.txt` file with the IGNs of everyone in the guild.

Next, run python app.py and open the website at `http://127.0.0.1:5000`. Upload the IGNs list and the recording.

`log.txt` will have the unfiltered results of everything that gets parsed. `results.csv` will have results filtered to only have **IGN | Culvert | Flag Race**.

`errors.csv` will have IGNs that could not be matched for debugging and manual solving.

