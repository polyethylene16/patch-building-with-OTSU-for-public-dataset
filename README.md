# patch-building-with-OTSU-for-public-dataset
This project is an implementation of the OTSU algorithm for masked segmentation of slide-level pathology image public datasets and generation of patches.
## Environment Configuration
    Python               3.7+
    numpy                1.21.5
    opencv-python        4.7.0.68
    openslide-python     1.2.0
    pillow               9.0.1
    matplotlib           3.5.1
    pytorch              1.12.0
    tqdm                 4.64.0
    
    
## Data Directory
Before running `patch1.0.py` the dataset needs to be deployed as follows：<br>

        ORIGINAL_DATA/
	         ├── slide_1.svs
	         ├── slide_2.svs
             ├── slide_3.svs
	         └── ...
             
## Result Directory
The execution results will be saved in the following structure: <br>
		
		PROCESSED_DATA/
		         ├── slide_1_20
			        ├── thumbnail
				       ├── mask.png
				       └── thumbnail.png
				├── 1_1.png
				├── 1_2.png
				└── ...
			 ├── slide_2_20
			        ├── thumbnail
				       ├── mask.png
				       └── thumbnail.png
				├── 1_1.png
				├── 1_2.png
				└── ...
			 └── ...

## Update
* 2023/01/11   Version1.0  |  Completing the slicing of tissue region by leveraging OTSU algorithm
