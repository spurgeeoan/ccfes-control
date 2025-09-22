## Edit 9/19
# Purge all CCFES, Create CH+FES + Interface
1. delete old days/versions of files
2. clean up this README as you delete things
3. no more EMG
4. 


branches
- aug28branch: CCFES control repository, as-is
- P24-control: edit beginning 9/19
- CH-P24-control: repo for project


## Upon startup
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass 
conda activate i24setup2 
cd ccfes-setup 
cd ccfes-setup-7-29
$env:PYTHONPATH="Y:\Hasomed Code\HasomedSetup13\ScienceMode4Python"

cd ..
cd ..
cd examples
cd dyscom

# if 'no module named examples'
$env:PYTHONPATH="Y:\Hasomed Code\HasomedSetup13\ScienceMode4Python"

# device manager from powershell - devmgmt.msc 

# check COM ports
# List all COM ports
Get-WmiObject Win32_SerialPort | Select-Object Name, DeviceID, Description


## keep-folder 
- csv_files folder - where all the csv files are saved to
- dyscom_runlive.py - Alisa's version of ScienceMode4Python dyscom files to run data collection from the I24 live, then save to a CSV file 
    - ver. 5 - OG code, + gain settings
- midlevel_runlive.py - scienceMode4Python version of pyScienceMode P24 runlive code (2 channels)
    - ver. 2 - changes plotting functions to fastplotlib.utils functions



