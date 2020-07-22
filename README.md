# photos-anomaly
Takes in a bunch of unorganised folders containing photos and structures them into folders based on location data and create date.

Purpose of this project is to handle the crazy amout of images i take/receive on my phone. I need this to be tuned and automated enough i just put in a bunch of photos in a folder and it automatically classifies them.

This tool should :
1. Takes input of a bunch of folders
2. Recursively scan them and extract all data in images into a json
3. Run an <<algorithm>> to classify these images into a structured directories
4. Present the assumed structure to user, allow user to modify the structure - dry run
5. allow option to execute said restructuring

Something else this tool can handle:
1. Detecting duplicate images. Using existing library of available images, ensure no duplicate images are placed in folders.
2. Detecting blurry images - user can specify which images to click


# <<algorithm>>
  This is mostly undefined as of yet. A basic idea is to use a classification algorithm, like k means.
  Data points can be - 
  1. folder name - this is probably album name. all folders kept in initially the same folder shall remain in the same folder, unless otherwise specified.
  2. geo location data - To automatically name albums based on vacation location.
  3. Photo taken by - to seperate images taken from different cameras/phones - This can be useful when automatically classifying images, but otherwise should be controlled manually.
  
