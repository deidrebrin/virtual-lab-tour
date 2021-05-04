# virtual-lab-tour

Simple virtual lab tour with 360 photos and videos using Pannellum

## Adding hotspots (informational points/links)

Turn on hotSpotDebug - this enables you to get the pitch and yaw from the console

## Adding scenes (new labs)

- Create new directory for the lab and add the 360 image along with any other items that might be displayed in the hotspots
- Add new scene with hotspots to the tour.html file (simplest to copy one of the previous labs and edit)
- Turn on hotSpotDebug to facilitate placing hotspots and initial view
- Open tour.html in a web browser and confirm the 360 image is loading properly
- Open developer tools -> console
- Pan and move the image so that the crosshairs in the center is lined up with where you would like to place an informational hotspot or a move button. Click and copy the pitch & yaw from the console (center) into the appropriate hotspot in tour.html
  - For informational popups, use the "info" type hotspot
  - For move buttons, use the "scene" type hotspot
- To set the initial view, get the appropriate pit, yaw, & hfov from the console and copy into the start of the scene object in tour.html
- Edit the text in each hotspot (use basic html and try to keep short - you can always link to another page)
- Save and reload to view your edits
