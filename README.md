# DC Offset Visualizer

This program is essentially written to easily obtain the DC offset of a short circuit curret from a Power System Event Recorder (Disturbance Fault Recorders) on an ASCII COMTRADE file. This can be COMTRADE Files from any Relay, or device so long as it is ASCII and not the Binary format.

Lots of work is still planned and being done on this project and it is in its infancy. 
The end goal is for this program to analyse such a file, detect a Power System Transmission line fault and get the relevant Currents Voltages and Power from the Oscillographic recordings and populate the data on a Spreadsheet. 
Python - pandas libraries are to be included in the Future but as of now OpenpyXL and csv_read is used. 

All Fault detection and Mathematics happens in the Script: faultdetect.py
DCRUNClass is the script where the program essentially runs and executes. It is dirty and ugly programming but works to to the basic tasks. 
Lots of cleanup still needs to happen.

This Program used a Discrete Fourier Transform to obtain the necessary data. You can refer to this as Phasors or Fourier-RMS values
DC value is the value at 0Hz
50Hz value is the Fundamental frequency and can be 60Hz in the Americas
1-nth harmonics will be multiples of 50Hz. 

Future Plans include:
Output window formatted with readability
Complete Spreadsheet population of all results
better fault detection
Basic Impedance plots

Original Author: [commander-apemanx](https://github.com/commander-apemanx/Comtrade-DC-Offset)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

PYTHON3
and 
packages

What things you need to install the software and how to install them

```
Give examples
```

### Installing

INSERT INSTRUCTIONS HERE

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc


