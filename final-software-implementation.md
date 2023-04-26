# Final Software Implementation


## C Source Code
Below are all the source files used for the PIC code:
### Main file
<script src="https://emgithub.com/embed-v2.js?target=https%3A%2F%2Fgithub.com%2Fegr314-team202%2Fproject-code%2Fblob%2Fmain%2Fpic%2FTeam202-PIC-Code%2FTeam202-PIC-Code.X%2Fmain.c&style=default&type=code&showBorder=on&showLineNumbers=on&showFileMeta=on&showFullPath=on&showCopy=on"></script>

### I2C Driver
We had to modify code we found to build an I2C driver for the PIC24 as it was not compatible with the existing I2C examples we had.
<script src="https://emgithub.com/embed-v2.js?target=https%3A%2F%2Fgithub.com%2Fegr314-team202%2Fproject-code%2Fblob%2Fmain%2Fpic%2FTeam202-PIC-Code%2FTeam202-PIC-Code.X%2FeepromI2C.c&style=default&type=code&showBorder=on&showLineNumbers=on&showFileMeta=on&showFullPath=on&showCopy=on"></script>
<script src="https://emgithub.com/embed-v2.js?target=https%3A%2F%2Fgithub.com%2Fegr314-team202%2Fproject-code%2Fblob%2Fmain%2Fpic%2FTeam202-PIC-Code%2FTeam202-PIC-Code.X%2FeepromI2C.h&style=default&type=code&showBorder=on&showLineNumbers=on&showFileMeta=on&showFullPath=on&showCopy=on"></script>

### Project Functions
Most of our main functionality is abstracted into the project functions files, to keep the `main.c` file clean.
<script src="https://emgithub.com/embed-v2.js?target=https%3A%2F%2Fgithub.com%2Fegr314-team202%2Fproject-code%2Fblob%2Fmain%2Fpic%2FTeam202-PIC-Code%2FTeam202-PIC-Code.X%2Fproject_functions.h&style=default&type=code&showBorder=on&showLineNumbers=on&showFileMeta=on&showFullPath=on&showCopy=on"></script>
<script src="https://emgithub.com/embed-v2.js?target=https%3A%2F%2Fgithub.com%2Fegr314-team202%2Fproject-code%2Fblob%2Fmain%2Fpic%2FTeam202-PIC-Code%2FTeam202-PIC-Code.X%2Fproject_functions.c&style=default&type=code&showBorder=on&showLineNumbers=on&showFileMeta=on&showFullPath=on&showCopy=on"></script>