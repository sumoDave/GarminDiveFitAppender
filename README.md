# GarminDiveFitAppender
GarminDiveFitAppender is a java utility that combines multiple sequential dives into a single dive activity.
It re-calculates summary data such as total dive time, temperature, depth, dive number and surface interval to display nicely in Garmin Connect web application, and in the Garmin Dive App.

Instructions:
1. Export dives to be combined in FIT format (export original). Note: Keep these files somewhere safe as the originals.
2. Unzip the dives and place the .fit files into a folder.
3. Unzip the GarminDiveFitAppender utility.
4. Drag and drop the dives onto the batch file to process into a combined dive.
   * Alternatively, in a command window, run the command "java -jar GarminDiveFITTool.jar -f <path to dive 1> <path to dive 2>".
6. Delete the original dives from Garmin Connect, and import the combined dive.

Notes:
1. Only tested with Single Gas dives recorded on a Descent G1.
2. Limited Tank Integration support - only tested with single transmitter, on single dataset.

Help:
```
Utility requires at least 2 fit files to append.
usage: java -jar GarminDiveFITTool.jar -f <fit files> [-h] [-l]
 -f,--fitFiles <fit files>   fit files to append.
 -h,--help                   Print usage.
 -l,--lap                    encode file with lap per file.
``` 
