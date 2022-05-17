## T-Rex Dinosaur Run

For my final project I attempted to recreate the game that displays when you lose internet connection while on google chrome.

The game was designed as a fun way to pass time while you were waiting for your computer to connect to the internet.

I attempted to recreate this by utlizing a version already designed by Sam Rose. The github for his project is located [here](https://github.com/samrose3/trex-runner)

The first major issue that I ran into when doing this project was that Sam had designed his code using a different board and a different constraint file type.

His vhdl code used a UCF constraint file rather than XDC, so my first objective was to create an XDC file based off this UCF file to run the code. 

After doing this I also had to remap some of the buttons that controlled the program, mainly the reset and jump buttons, which I remapped to BTNL and BTNC, respectively. 

After doing all this I was hoping the project would've been finished, but unfortunately it was not. I ran into my next error, which was that when streaming to a monitor the monitor's gave me the error "Frequency out of range"

I have not been able to fix this error yet, but I do believe that once I do the project will hopefully work.
