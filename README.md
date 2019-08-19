# Metal3DPrinter
This project is the LabView GUI and Control system of the metal 3D printer at Fab Lab. The system provides a GUI for users to monitor and control the instruments.  

## Prerequisites

The ***development environment*** requires following:

- LabView 2018 
- NI LabView VISA 
- NI DAQ-mx 
- Microsoft Visual C++ 2019 (Phase 2) 
- Python 3.7.9 (Phase 2) 

The ***run-time environment*** requires following: 

- LabView 2018 run-time 
- NI LabView VISA 
- NI DAQ-mx 
- Microsoft Visual C++ 2019 run-time (Phase 2) 
- Python 3.7.9 (Phase 2) 

## Installing

1. Right click the empty space with in the folder where you want to put the files and open the Git Bash.
2. Within the Git Bash, type command: `git clone https://github.com/uw-loci/Metal3DPrinter` and hit `ENTER`
3. Open LabView and click `File -> Open Project` and select `Master_Control.lvproj`

## Architecture

This program adopt a Microkernal Architecture. All subsystems are standalong and can function individually without the main program. A failure of any subsystems will NOT interrupt the normal execution of the main program. Running the main program will automatically call the other sub VIs and all subVIs run concurrently. 

Global VIs connect each subVI to facilitate data communication. 

## Authors

- **Yuanzhe Liu** - *2019-2020*
