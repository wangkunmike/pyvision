## PyVision Computer Vision Toolkit
    by David Bolme

As of August 2014, PyVision is now hosted at github:
    <http://github.com/bolme/pyvision>

For additional documentation please see the github wiki:
    <http://github.com/bolme/pyvision/wiki>

PyVision is a object-oriented Computer Vision Toolkit (**BSD Licenses**) 
that is designed to allow the rapid prototype and analysis of computer 
vision algorithms.  Using python as a foundation this package provides 
a simple framework that unifies the Matlab like functionality of 
scipy/numpy, Open Computer Vision Library (opencv), and other vision 
and machine learning software packages.  In addition PyVision provides 
a set of analysis tools that allows the researcher to evaluate there 
algorithms in python or to export those results in csv format for 
analysis in Excel, R, or SAS.

PyVision is a collection of computer vision algorithms that I have implemented 
as part of my Ph.D. face recognition research.  The purpose of the library is 
to provide a set of utilities that interface with common computer vision and 
machine learning libraries that will allow rapid vision algorithm prototyping. 
For example the current implementation has an image class which will easily 
translate image data between PIL, numpy array, and opencv formats.

### Overview
Currently, PyVision contains a set of popular computer vision algorithms 
including: 

- canny edge detection 
- harris corner detection
- viola and jones face detection
- support vector machines and other classifiers
- image normalization primitives
- Difference of Gaussian ROI detection
- Genetic Algorithm
- Phase Correlation
- Eye Detection (ASEF and MOSSE Filters)
- PCA and LDA analysis
- PCA Face Recognition
- Image Affine Transform
- Video Stream Processing

Pyvision also has a set of built in analysis tools (based on scipy) for 
analyzing and testing vision algorithms.  This includes a simple image 
annotation frame work formal statistical analysis that produces confidence 
limits and p-values, classes designed for face detection and face recognition 
tests, and a table class which allows experiment data to be accumulated and 
then exported to csv, txt, or tex formats.  PyVision also has a simple GUI 
(based on opencv and wxpython) which allows for the easy creation of live 
demos.

My goals for releasing this library is to provide this 
toolkit to other computer vision researchers.  I would also like to have a 
place where other researchers contribute their code, and I could use some 
help making the toolkit multi-platform.  The current version is focused on 
face recognition, and I would like some help expanding the library to other 
areas of computer vision and machine learning.

This library is a set of useful python classes for quickly constructing 
and analyze computer vision systems.  The library provides a set of 
easy to uses object and algorithms that can be used to quickly prototype 
new vision algorithms. 

This library contains vision algorithms that should be of general use 
to many people.  As best as possible I will include training configurations,
sample code, and unit tests to aid others in reusing the code.

My current research is focused on face recognition so much of the active
development will be related that area.  Contributions in other areas of 
research are welcome including: Object Recognition, Biological Vision, 
Multiview Geometry, etc.

### Dependencies

- PIL
- scipy
- numpy
- scikit learn (As of pyvision 2.0)
- scikit image (As of pyvision 2.0)
	

### Recommended
- OpenCV (optional)


### Features:
	
- Python based for rapid prototyping.
- Common data types with easy conversion.
- Automatically tuned or easy to configure algorithms.
- Numerical support from scipy.
- Image support from PIL.
- Pretrained algorithms for common tasks.
- Python and R based algorithms analysis.
- Unit tests for algorithm verification.
- Sample code and tutorials.
- Save and load configurations with python's pickle.
- Simple interfaces to third party software: OpenCV and libsvm.

** Notes: **
	Image.asOpenCV() - Requires fix to opencv bug #1618474 included in cvs on 
	    Jan 25, 2007 18:19:21 UTC by rstanchak
	
### Releases:

* 1.3.0 - OpenCV is no longer required.  This makes setup easier.  Better support for "pip install pyvision_toolkit".
* 1.2.0 - Support for Python 3 and OpenCV 3
* 1.1.0 - It has been a while since the last release.  OpenCV has improved 
            recently and has become more stable with improved python bindings.  
            As a result PyVision is adapting to use OpenCV for much of its
            core functionality.  In general OpenCV tends to be faster and 
            more accurate for common image processing functions than scipy or
            PIL.  Additionally OpenCV will be used in the future for machine
            learning algorithms.  The Video Task Manager (VTM) framework is 
            improving for quickly developing video processing pipelines.  
* 1.0.0 - Many interface things have been cleaned up.
            Function arguments that are keywords have been change and may not 
            work as in previous version.  These include: buffer, type, filter,
            iter. All warnings and errors from the code analysis have been 
            fixed.
* 0.8.1 - Released in July 2010. This is the last release before a major 
            upgrade and the last version to support OpenCV 1.0 with the swig 
            bindings.
* 0.8.0 - Released in June 2009.  This was primarily to support FaceL.

