# Instructions for updating the virtual lab tour

You will want to test your updates to the virtual lab tour locally on your computer before uploading to the server. You can do so by using XAMPP to set up a local server on your computer that will simulate the environment.

## Local setup

- Clone the [repository](https://github.com/deidrebrin/virtual-lab-tour) from GitHub
- Install XAMPP from [here](https://www.apachefriends.org/index.html)
- Open the XAMPP directory and find the htdocs directory
- Copy the "virtual-lab-tour" directory into the htdocs directory
- Open the XAMPP control panel and start Apache
- Open a browser and navigate to localhost/virtual-lab-tour/
  - The tour should load!

## Editing or adding a lab

- If you are adding a new lab, create a new directory (do not include spaces in the directory name) and add the 360 image along with any other images or videos that might be displayed in the hotspots
- Edit the tour.html file using the template.html file (in the docs directory) as a guide (the comments denoted by "//" throughout this file describe how to edit each section)
  - Ensure that all of the images or videos you are linking to in the information popups are in the appropriate lab directory and you have the correct path and filename for them
- Add a new scene with hotspots to the tour.html file (simplest to copy one of the previous labs and edit)
  - Recommend using [Sublime text](https://www.sublimetext.com/) if you haven't used a text editor before
- Open localhost/virtual-lab-tour in a web browser and confirm the 360 image is loading properly
- To add informational popups, use the "info" type hotspot
- To add move buttons, use the "scene" type hotspot
- To set the initial view, get the appropriate pit, yaw, & hfov from the console and copy into the start of the scene object in tour.html
- Edit the text in each hotspot (use basic html and try to keep short - you can always link to another page)

- If you are updating an existing lab, navigate to the appropriate directory and add any new images, videos, or content as needed.

  - Open the tour.html file and update the entry for that lab as desired

- Save and reload to view your edits

### Getting the pitch and yaw for hotspots

- You can turn on the "hotspotdebug" option by entering True in the tour.html file
- Now when you load the file in the browser, you will have a point with crosshairs in the center of the page
- Open developer tools in your browser and select the Console tab
  - Firefox: Ctrl + Shift + I or F12 on Windows or Cmd + Opt + I on macOS
  - Chrome: Shift + CTRL + J (on Windows/Linux) or Option + ⌘ + J (on macOS)
  - Safari: Cmd + Opt + J (Mac)
- Now when you click on the page, the pitch and yaw will be printed to the console - both the point you clicked and the centerpoint (where the crosshairs are)
- Copy the numbers to the hotspot in the tour.html file - two digits to the right of the decimal point is sufficient

### Viewing the changes

Once you have the index.html file edited as desired, you can open the site running locally through XAMPP by going to localhost/virtual-lab-tour/index.html

### Notes

You can turn off Apache when you're finished editing, just remember to restart the server before you begin editing again or nothing will load.

## Uploading to the server

- Use the FTP credentials provided to access the virtual-lab-tour directory on the server
- Replace the tour.html file and any edited files
- Upload any new directories and files
- Confirm that the site has updated - [Virtual Lab Tour](https://dal.ucla.edu/virtual-lab-tour/)
