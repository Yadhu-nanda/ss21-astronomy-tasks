# Task for Hands-On Astronomy

### Deadline: 14/07/2021 11:59 PM

## Rules

1. Use only commands, functions, datatypes taught in the sessions till present.
2. You are free to use whatever resource to learn about the subject of task.
   Please avoid plagiarism - the task is for you to learn, not for us to evaluate
   you.
3. Refrain from using pre-existing libraries/functions/other structures unless asked to in the assignment.
4. Your submission should be a Jupyter Notebook with all the code pertaining to each task done sequentially.

## Tasks
1. Download the FITS file present in the `data` folder.
2. Read the file using `astropy.io.fits` module and store the returned object.
3. Find the number of HDUs present in this FITS file.
4. Read the primary header and make a list containing the answer to the following questions.
   1. What is the length of axis 3?
   2. What is the axis 3 supposed to be?
   3. What are the units of axis 3?
   4. What is the name of the telescope?
   5. What is the name of the observer?
5. Extract the data from the primary HDU. For the first slice of this data, find the maximum and minimum pixel value along with the standard deviation of this data.
6. Look into the arguments of the `pyplot` function `imshow`. Use the pixel values obtained above to limit the colour scaling of `imshow`. Use `cmap='gray'` while plotting the image. (Make the plot look nice by appropriately choosing the figure size and using labels.)
7. 'Stack' every 5th slice (slice 5, 10, 15...) of the original data. This can be done by simply summing the slices (arrays) together. Plot this new dataset by repeating task 5 and 6. 
8. Create a function that plots the 'Altitude' of a celestial object 12 hours after a given time. Assume you are located at IITM, like I did during the session and the coordinates of the object are knowing in some other coordinate system. You should need only two arguments, `coordinates` of the object and the desired `time` of observation.

## Submission procedure
1. Fork this repository. (If you have already forked ignore this step.)
2. Clone the forked repository to your system. And go to the cloned repository directory. (If you have already cloned ignore this step, but _do_ sync it.)
3. Sync your fork with the original repo, and pull changes before proceeding further.
4. Place your final submission (`.ipynb` files only) in the `tasks` folder with the name format `rollnumber` (name should be all lowercase only). 
5. Sync your fork with the original repository, and pull changes from your fork to the cloned local repository, before proceeding further.
6. Make sure not to affect any files in other directories.
7. Add all the changes, and commit them.
8. Create a pull request with title format `rollnumber_name_astro`. It should be in all lowercase, and replace spaces in name with `-`. `name` is your name, not your GitHub username.
9. And that's it!