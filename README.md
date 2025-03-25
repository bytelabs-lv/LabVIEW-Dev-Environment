# Bytelabs LabVIEW Development Environment (Byte-LVDevEnv)
**LabVIEW VIPM configuration management for projects, PIP style**

## Description
**This library creates a tool in the LabVIEW tools palette, which can be found under Bytelabs > DevEnvironment > Installer.**
<br>
This tool allows to select an input version specification file (similar to a requirements.txt file),
with package information features (as described below).
<br><br>
It also allows to select a local (or network) folder where you and your team store private .vip packages, which will
also be used for packages lookup.
<br><br>
Each project can then have its package.txt file, specifying the required packages and their acceptable versions.
<br>
The tool will then configure the environment, installing required packages from the web or from your local folder,
always selecting a compatible version, even upgrading or downgrading when needed, leveraging on VIPM's APIs.

## input file specifications
Input file (packets.txt, usually but not strict) have the following characteristics
* Can set a required package, without specific version > the most updated version will be installed
* Can set a required package, with a minimum (or maximum) version > in this case, if the packet is already installed and has a compatible version, it will not be touched. Otherwise the most updated allowed version will be installed
* Can set a required package, with a minimum and a maximum version > same as above, within the allowed version range
Refer to the [Examples folder](examples/) to see a version of this file

