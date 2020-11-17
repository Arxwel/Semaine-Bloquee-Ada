# Antiviros



## About

Antiviros is a computer version of the [Antivirus board game](https://www.smartgames.eu/uk/one-player-games/anti-virus) made in Ada. At the moment, it has only 20 challenges available.

It was created as a school project during the first year of my Associate's degree at IUT2 Grenoble.

## Installation

The game has been tested on Linux and should run on MacOS. I don't think windows can run it because of the graphical library.

### Ada Libraries

The project use a custom graphical library based on x11, and some other libraries. In order to launch the game you will need to download them.



1. First, download the following archive.
   
   ```bash
   wget https://romain-pasdeloup.fr/download/AdaLib.zip
   ```

2. Then, extract it. 
   
   ```bash
   unzip AdaLib.zip
   ```

3. You're done! You are free to put it in the directoy of your choice.



### Game

To play the game, download the content of this repository. To compile the program you must have GNAT compiler installed on your system.

1. Update LD_LIBRARY_PATH to add our custom libraries
   
   ```
   export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:PATH_TO_LIBRARY/lib
   ```
   
   Where you replace ''PATH_TO_LIBRARY" with the path where the libraries you previously downloaded can be found.
   
   This step is mandatory to tell the compiler where it can found them.

2. Compile
   
   A bash script named ```compile.sh``` has been made to simplify the compilation.
   
   Before running it, make sure you have the right permissions:
   
   ```bash
   chmod u+x compile.sh
   ```

3. Play!
   
   Once you have compiled everything, you're ready to go!
   
   You should have two executables generated by the compilation: ```antivirus``` and ```avgraphique``` .
   
   The first one is the textual version and can be played in a terminal. 
   
   The second one is the graphical version.
   __Note__: When you open a new terminal, you must do the export specified in step 1. before playing.