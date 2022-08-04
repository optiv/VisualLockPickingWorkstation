<H1>Visual Lock Picking Workstation</H1>
By: Doug Rogahn


The Visual Lock Picking Workstation is a Raspberry Pi enclosure which makes it possible to capture live
video from a cutaway lock. It is intended as an instructional device which can be used to display the
inner workings of a lock while teaching lock picking.

The 3d model file is available on the Optiv git repository at the following link:
https://github.com/optiv/VisualLockPickingWorkstation.git

Required Components
* Raspberry Pi 3
* Raspberry Pi Camera module (you will need to unscrew the lenses to focus)
* Light Ring for Raspberry Pi Camera (I suggest the Bright Pi)
* Cutaway Lock Core
* 3d printed enclosure


![](https://j.gifs.com/gpPyp9.gif)

Command line for displaying live video. This can also be added to a startup script so that it
automatically starts every time the pi boots.

```Raspivid -t 0 -vf -w 1920 -h 1080 -fps 30 -rot 270```
