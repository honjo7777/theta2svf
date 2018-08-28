# theta2svf
The R program, "theta2svf_basic_revised.R"
can convert Theta image (equidistant cylindrical projection) to fisheye image (equidistant and equal-area projection) and
binarize the images to calculate sky view factor.  
Theta can be used as the fisheye lens camera by the method of this program.

The following input file is used.  
  example.jpg: Theta image (equidistant cylindrical projection) used as input file.  

Following output files are made.  
  example_dist.png: fisheye image of equidistant projection  
  example_dist_bi.png: binarized bw fisheye image of equidistant projection  
  example_area.png: fisheye image of equal-area projection  
  example_area_bi.png: binarized bw fisheye image of equal-area projection  
  example_area_svf.txt: sky view factor calculated from binarized fisheye image of equal-area projection  
  
 To run the program, place the "theta2svf_basic_revised.R" and "example.jpg" in the same folder.  
   In "theta2svf_basic_revised.R", following line should be changed  
   Please change the directry in line 9 like, "setwd("/Users/honjo/Desktop/test_folder")" which is the folder name for test.  
   
 Also the following values of the parameter are changed if necessary.  
   xth<-0.6 #threshold value in making binary images  
   #rgb ratio  
   r_ratio<-1  
   g_ratio<-1  
   b_ratio<-1  

copyright 2017(c) Tsuyoshi Honjo
