Total root length and root length in diameter classes  
by Ryosuke TAJIMA  
=====================
  
  
# Download ImageJ and this ImageJ macro
## ImageJ  
https://imagej.nih.gov/ij/  
https://imagej.net/software/fiji/downloads  
  
## ImageJ macro  
"RootLength.txt" in this repository  
  
# Install macro to ImageJ  
In ImageJ, select ImageJ macro "RootLength.txt" ("Plugins>Macros>install..."").  
Check "Plugins>Macros..."".  
You can find two added macros: "TotalRootLength" and "RootLength_in_DiameterClasses".  
  
# Setting  
## Create folders
In mac, create two folders named "roots" and "dimameters" in home folder, which has House icon.  
In Windows, create two folders named "roots" and "dimameters" in user folder (C:\Users\******).  
  
## Set dpi
### Mesuring total root length
If you need to use the images except for 400 dpi, change the value in L14.  
For example,  
  
L14: dpi = ~~400;~~ 300;  
  
### Mesuring root length in dimameter classes.
This macro only supports 400 dpi image and five dimater classes (<0.1, 0.1-0.2, 0.2-0.5, 0.5-1.0, and >1.0 mm)  
  
## Set the image cropping
If you need to omit the frame of the case from the image, change the code in L3-6.  
For example,  
  
L3: x = ~~0;~~ 100;  
L4: y = ~~0;~~ 150;  
L5: width = ~~getWidth ();~~ 1500;  
L6: height = ~~getHeight ();~~ 2000;  
  
or modify and use L8.
  
# Measure the length  
Put all images in the "roots" folder.  
Click "TotalRootLength" or "RootLength_in_DiameterClasses".  
  
# Save the data
After estimation, save "Log" as a txt file.  
You can open the file as a space-delimited file in Excel.  
The unit of root length is centimeter.  
  
# References
When you use this macro in your paper, please refer to two papers.  
  
Tajima, Ryosuke and Kato, Yoichiro. 2011. Comparison of threshold algorithms for automatic image processing of rice roots using freeware ImageJ. Field Crops Research. 121: 460-463.  
  
Tajima, Ryosuke and Kato, Yoichiro. 2013. A Quick Method to Estimate Root Length Distribution in Diameter Classes by Using Freeware ImageJ. Plant Production. Science. 16: 9-11.  
  
# Licence
https://github.com/blukaniro/rootmeasure/blob/master/LICENSE
  
  
  
Thanks.  