# mammoreplicator
This repository contains the source code of the _mammoreplicator_ software described in the article: __Andreu Badal, Matthew Clark, Bahaa Ghammraoui, "Reproducing two-dimensional mammograms with three-dimensional printed phantoms", Journal of Medical Imaging 5, p. 033501 (2018)__. The software was initially introduced at the SPIE Medical Imaging 2016 conference.

The _mammoreplicator_ software implements a simple, easily reproducible methodology to create 3D phantoms that replicate the attenuation profile observed in real 2D mammograms.
The software processes an input raw mammography image to estimate the amount of x-ray attenuation at each pixel, and outputs a triangle mesh object that encodes the observed attenuation map.
Each pixel in the input image is transformed into a column of material tilted towards the direction of the x-ray focal spot, so that the projection of the column covers exactly the area of the original pixel.
The conversion from the observed pixel gray value to a column of printed material with equivalent attenuation requires certain assumptions and knowledge of multiple imaging system parameters, such as x-ray energy spectrum, source-to-object distance, compressed breast thickness, and average breast material attenuation.
The methodology used in this software is similar to that introduced by Caldwell and Yaffe in 1990 (https://doi.org/10.1118/1.596506).



## Disclaimer

This software and documentation (the "Software") were developed at the Food and Drug Administration (FDA) by employees of the Federal Government in the course of their official duties. Pursuant to Title 17, Section 105 of the United States Code, this work is not subject to copyright protection and is in the public domain. Permission is hereby granted, free of charge, to any person obtaining a copy of the Software, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, or sell copies of the Software or derivatives, and to permit persons to whom the Software is furnished to do so. FDA assumes no responsibility whatsoever for use by other parties of the Software, its source code, documentation or compiled executables, and makes no guarantees, expressed or implied, about its quality, reliability, or any other characteristic. Further, use of this code in no way implies endorsement by the FDA or confers any advantage in regulatory decisions. Although this software can be redistributed and/or modified freely, we ask that any derivative works bear some notice that they are derived from it, and any modified versions bear some notice that they have been modified.
