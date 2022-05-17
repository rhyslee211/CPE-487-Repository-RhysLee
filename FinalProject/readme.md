## T-Rex Dinosaur Run

For my final project I attempted to recreate the game that displays when you lose internet connection while on google chrome.

The game was designed as a fun way to pass time while you were waiting for your computer to connect to the internet.

The game has 2 main parts to it: The dinosaur, who the player controls, and the enemies, the cacti and pterodactyls, who if touch the dinosaur, end the game.

![](/images/googletrexrun.png)

I attempted to recreate this by utlizing a version already designed by Sam Rose. The github for his project is located [here](https://github.com/samrose3/trex-runner)

His version of the game looked like this

![](/images/trex_runner_02.png)

The first major issue that I ran into when doing this project was that Sam had designed his code using a different board and a different constraint file type.

His vhdl code used a UCF constraint file rather than XDC, so my first objective was to create an XDC file based off this UCF file to run the code. 

After doing this I also had to remap some of the buttons that controlled the program, mainly the reset and jump buttons, which I remapped to BTNL and BTNC, respectively. 

After doing all this I was hoping the project would've been finished, but unfortunately it was not. I ran into my next error, which was that when streaming to a monitor the monitor's gave me the error "Frequency out of range".

The next error I experienced was a "frequency out of range" error on the monitors. The problem for this was that the original code was made to be run on 640 by 480 monitors, but I used 800 by 640. After changing a few numbers to new values, the video was able to display.

Once the display started working the game was able to be played. The BTNC button would make the dinosaur jump and the BTNL would reset the game. The game also automatically reset after the dinosaur died.

[Here is a link to a video of the working project.](https://www.youtube.com/watch?v=qGho2Cwx7Rg)

# Instructions

To run the T-Rex Runner project, create a project folder and download all the files and add the VHD files as sources, and the XDC file as a constraint.

Then run synthesis, run implementation, and then generate a bitstream.

Next connect a 800 by 640 monitor to the board through a VGA connection. Then program the board with the bitstream.
