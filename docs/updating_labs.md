# Instructions for updating the virtual lab tour

You will want to test your updates to the virtual lab tour locally on your computer before uploading to the server. You can do so by using XAMPP to set up a local server on your computer that will simulate the environment.

## Local setup
- Clone the [repository](https://github.com/deidrebrin/virtual-lab-tour) from GitHub
- Install XAMPP from [here](https://www.apachefriends.org/index.html)
- Open the XAMPP folder and find the htdocs folder
- Copy the "virtual-lab-tour" folder into the htdocs folder
- Open the XAMPP control panel and start Apache
- Open a browser and navigate to localhost/virtual-lab-tour/index.html
  - The tour should load
- Open the htdocs/virtual-lab-tour folder again and open index.html in a text editor (recommend using Sublime text or VS Code)
- Edit the index.html file using the template.html file (in the docs folder) as a guide (the comments denoted by "//" throughout this file describe how to edit each section)

## Getting the pitch and yaw for hotspots
- You can turn on the "hotspotdebug" option by entering True
- Now when you load the file in the browser, you will have a point with crosshairs in the center of the page
- Open developer tools in your browser and select the Console tab
  - Firefox: Ctrl + Shift + I or F12 on Windows or Cmd + Opt + I on macOS
  - Chrome: Shift + CTRL + J (on Windows/Linux) or Option + ⌘ + J (on macOS)
  - Safari: Cmd + Opt + J (Mac)
- Now when you click on the page, the pitch and yaw will be printed to the console - both the point you clicked and the centerpoint (where the crosshairs are)
- Copy the numbers to the hotspot in the index.html file - two digits to the right of the decimal point is sufficient

## Viewing the changes
Once you have the index.html file edited as desired, you can open the site running locally through XAMPP by going to localhost/virtual-lab-tour/index.html 


## Notes:
You can turn off Apache when you're finished editing, just remember to restart the server before you begin editing again or nothing will load.