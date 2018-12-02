3DPeS Snapshots for ReIdentification and orientation estimation:

RGB folder contains appearance images, MASK folder contains silhouette masks.
THE MASKS WERE EXTRACTED AUTOMATICALLY, they probably contains numerous errors.
The file 3dpes_train.al contains the following ground truth data:
-Bounding box of the person
-Orientation class (see image Classi.jpg)

3dpes_train.al file structure:

<annotationlist> 														//header

<annotation> 															//begin of image data
<image><name> 3DPes/RGB\100_3_FRAME_26_RGB.bmp</name></image>  			//image
<annorect>																//ground truth
<x1>0</x1>																//bounding box
<y1>0</y1>
<x2>41</x2>
<y2>105</y2>
<silhouette><id>6</id></silhouette>										//orientation class
</annorect>																//end ground truth
</annotation>															//end image data
...
...
</annotationlist>														//end file


File names:

100_3_FRAME_26_RGB.bmp corresponding mask is 100_3_FRAME_26_MASK.bmp
The first number is the person ID, 100 in this example. 
Same number = same person. Different number = different person :-) .

If you use this dataset please cite:

@inproceedings{baltieri2011_308,
	author = {Baltieri, Davide and Vezzani, Roberto and Cucchiara, Rita},
	title = {3DPes: 3D People Dataset for Surveillance and Forensics},
	booktitle = {Proceedings of the 1st International ACM Workshop on Multimedia access to 3D Human Objects},
	volume = {},
	number = {},
	year = 2011,
	month = nov,
	pages = {59--64},
	address = {Scottsdale, Arizona, USA},
}

@inproceedings{baltieri2011_305,
	author = {Baltieri, Davide and Vezzani, Roberto and Cucchiara, Rita},
	title = {SARC3D: a new 3D body model for People Tracking and Re-identification},
	booktitle = {Proceedings of the 16th International Conference on Image Analysis and Processing},
	volume = {},
	number = {},
	year = 2011,
	month = sep,
	pages = {197--206},
	address = {Ravenna, Italy},
}

If you use the provided masks, please cite also:

@article{vezzani2011_295,
	author = {Vezzani, Roberto and Grana, Costantino and Cucchiara, Rita},
	title = {Probabilistic people tracking with appearance models and occlusion classification: The AD-HOC system},
	journal = {Pattern Recognition Letters},
	volume = {32},
	number = {6},
	year = {2011},
	month = apr,
	pages = {867--877},
}