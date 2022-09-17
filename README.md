# *FeatSet+*: Visual features from open Image Datasets

*Last Update: September 2022.*

***FeatSet+*** is a dataset with visual features (color, texture, and shape) extracted from 17 open image datasets from the Literature. *FeatSet+* supports different analyses involving machine learning, image analysis, and content-based image retrieval (CBIR). Moreover, the dataset can serve researchers seeking to solve problems related to the study of image features from different applications, such as emergency scenarios, medical cases, and object classification or recognition.

## Complete Description and Further Information

The *FeatSet+* database schema is the following:  

![FeatSet+ database schema](https://github.com/mtcazzolato/featset/blob/main/schema.png)  
  
Each dataset in *FeatSet+* follows the same schema, with (a) a metadata table containing the object identifier (OID), the filename (which is the same as the public dataset), and the set of classes (if any). The (b) set of FEM tables has the OID as a foreign key (FK), and every dimension of the feature vector is stored as a column. Additionally, \(c\) the Feature Equivalence Table provides the Feature Extraction Method (FEM) name, the feature ID, and the corresponding description of every visual feature provided by the FEM.  
  
The complete description of  *FeatSet+* is given in the work [\[Cazzolato *et al.*, 2022\]](https://sol.sbc.org.br/journals/index.php/jidm/article/view/2328/1975).  

## License Agreement and Citation Request:

*FeatSet+* is available for researchers and data scientists under the GNU General Public License. In case of publication and/or public use of the available data, as well as any resource derived from it, one should acknowledge its creators by citing **the following paper and the paper from which the original images were acquired** (see the references in the description of the datasets, bellow).
  
**Extended work:**

> [\[Cazzolato *et al.*, 2022\]](https://sol.sbc.org.br/journals/index.php/jidm/article/view/2328/1975) CAZZOLATO, M. T.;  SCABORA, L. C.;  ZABOT, G. F.; GUTIERREZ, M. A.; TRAINA-Jr, C.; TRAINA, A. J. M.. **FeatSet+: Visual Features Extracted from Public Image Datasets.** In the JIDM Special Edition on Datasets of the Journal of Information and Data Management, Brazil. Vol. 13, n. 1. DOI: 10.5753/jidm.2022.2328. 2022. 

Bibtex:  
```
@article{CazzolatoEtAl2022,
  author    = {Mirela T. Cazzolato and
               Lucas C. Scabora and
               Guilherme F. Zabot and
               Marco A. Gutierrez and
               Caetano Traina Jr. and
               Agma J. M. Traina},
  title     = {FeatSet+: Visual Features Extracted from Public Image Datasets},
  journal   = {Journal of Information and Data Management (JIDM)},
  volume    = {13},
  number    = {1},
  year      = {2022},
  url       = {https://doi.org/10.5753/jidm.2022.2328},
  doi       = {10.5753/jidm.2022.2328},
}
```

**Original work:**

> [Cazzolato *et al.*, 2021] CAZZOLATO, M. T.;  SCABORA, L. C.;  ZABOT, G. F.; GUTIERREZ, M. A.; TRAINA-Jr, C.; TRAINA, A. J. M.. **A Compilation of Visual Features Extracted from Public Image Datasets.** In the Brazilian Symposium on Databases - Dataset Showcase Workshop (SBBD-DSW), Virtual Conference, Brazil. 2021. (to appear)

Bibtex:
```
@inproceedings{CazzolatoEtAl2021,  
      author = {Mirela T. Cazzolato and 
                Lucas C. Scabora and  
                Guilherme F. Zabot and  
                Marco A. Gutierrez and  
                Caetano Traina-Jr. and  
                Agma J. M. Traina},
      title = {FeatSet: A Compilation of Visual Features Extracted from Public Image Datasets},
      booktitle = {Brazilian Symposium on Databases - Dataset Showcase Workshop (SBBD-DSW), Virtual, Brazil, October 4-8, 2021. (to appear)},
      pages = {1--12},
      year = {2021}
}
```


## Download Links

SQL-Scripts-Link: Click [here](https://drive.google.com/file/d/13EBm8_qQgMZ_96AJKTsOvX4TBLZcMbRl/view?usp=sharing) to download the SQL scripts used to load the data.  
CSV-File-Link: Click [here](https://drive.google.com/file/d/1_jXUkrMuRQLp0gBLuleJHbFxbiMWOkPg/view?usp=sharing) to download the CSV files with the data. 

# *FeatSet+* Datasets

Following, we provide the description of the image datasets composing FeatSet+:  

Index:  

[Dataset ds-BoWFire](#dataset-ds-bowfire)  
[Dataset ds-Flickr-Fire](#dataset-ds-flickr-fire)  
[Dataset ds-Mammoset](#dataset-ds-mammoset)  
[Dataset ds-LibraGestures](#dataset-ds-libragestures)  
[Dataset ds-Food5k](#dataset-ds-food5k)  
[Dataset ds-Flickr-FireSmoke](#dataset-ds-flickr-firesmoke)  
[Dataset ds-Covid19](#dataset-ds-covid19)  
[Dataset ds-COIL100](#dataset-ds-coil100)  
[Dataset ds-CUB-200-2011](#dataset-ds-cub-200-2011)  
[Dataset ds-Letters](#dataset-ds-letters)  
[Dataset ds-Cars](#dataset-ds-cars)  
[Dataset ds-Food-11](#dataset-ds-food-11)  
[Dataset ds-Dogs](#dataset-ds-dogs)  
[Dataset ds-DeepLesion](#dataset-ds-deeplesion)  
[Dataset ds-AwA](#dataset-ds-awa)  
[Dataset ds-MNIST](#dataset-ds-mnist)  
[Dataset ds-CompCars](#dataset-ds-compcars)  

---
---

## Dataset *ds-BoWFire*  

### Source:  
    University of São Paulo  
    Institute of Mathematics and Computer Science (USP-ICMC)  
    Database and Image Group (GBdI)  

### URL:
    https://bitbucket.org/gbdi/bowfire-dataset  

### Date of Collection:
    October 9th, 2020

### License:
    Creative Commons

### Brief Description:
    Images depicting fire incidents from emergency situations. The available features were extracted from the entire images of the dataset (train files). Every image has a label in L={fire, not fire}.
    For further information, please refer to the original source.

### Reference:
    @inproceedings{dsBowFire2015,
    author          = {Daniel Y. T. Chino and Letricia P. S. Avalhais and Jos{\'{e}} F. Rodrigues-Jr. and Agma J. M. Traina},
    title           = {BoWFire: Detection of Fire in Still Images by Integrating Pixel Color and Texture Analysis},
    booktitle       = {28th {SIBGRAPI} Conference on Graphics, Patterns and Images, {SIBGRAPI} 2015, Salvador, Bahia, Brazil, August 26-29, 2015},
    pages           = {95--102},
    publisher       = {{IEEE} Computer Society},
    year            = {2015},
    url             = {https://doi.org/10.1109/SIBGRAPI.2015.19},
    doi             = {10.1109/SIBGRAPI.2015.19},
    }
---
---
## Dataset *ds-Flickr-Fire*  

### Source:  
    University of São Paulo  
    Institute of Mathematics and Computer Science (USP-ICMC)  
    Database and Image Group (GBdI)  

### URL:  
    https://github.com/mtcazzolato/dsw2017  

### Date of Collection:  
    October 9th, 2020

### License:  
    Creative Commons  

### Brief Description:  
    Images acquired from Flickr, using tags related to fire to filter the information. Every image has a label in L={flame, not flame}.  
    For further information, please refer to the original source.

### Reference:  
    @inproceedings{dsFlikrFire2015,
        author          = {Marcos Vinicius Naves Bedo and Gustavo Blanco and Willian D. Oliveira and Mirela T. Cazzolato and Alceu Ferraz Costa and Jos{\'{e}} Fernando Rodrigues-Jr. and Agma J. M. Traina and Caetano {Traina Jr.}},
        editor          = {Slimane Hammoudi and Leszek A. Maciaszek and Ernest Teniente},
        title           = {Techniques for Effective and Efficient Fire Detection from Social Media Images},
        booktitle = {{ICEIS} 2015 - Proceedings of the 17th International Conference on Enterprise Information Systems, Volume 1, Barcelona, Spain, 27-30 April, 2015},
        pages           = {34--45},
        publisher       = {SciTePress},
        year            = {2015},
        doi             = {10.5220/0005341500340045},
    }
---
---
## Dataset *ds-Mammoset*  

### Source:  
    University of São Paulo  
    Institute of Mathematics and Computer Science (USP-ICMC)  
    Database and Image Group (GBdI)  

### URL:  
    https://bitbucket.org/gbdi/mammoset

### Date of Collection:
    October 9th, 2020

### License:  
    Creative Commons

### Brief Description:  
    Regions of Interest (ROIs) obtained from mammograms. Additional information, such as 'benign' and 'malignant' labels, background tissue and abnormality severity can be found in the original paper.
    For further information, please refer to the original source.

### Reference:  
    @inproceedings{dsMammoset2017,
        author          = {Oliveira, P. H. and Scabora, L. C. and Cazzolato, M. T. and Bedo, M. V. N. and Traina, A. J. M. and Traina-Jr., C.},
        booktitle       = {Proceedings of the Satellite Events of the 32nd Brazilian Symposium on Databases},
        title           = {{MAMMOSET: An Enhanced Dataset of Mammograms}},
        year            = {2017},
        pages           = {256--266},
        publisher       = {{SBC}}
    }
---
---
## Dataset *ds-LibraGestures*  

### Source:  
    Intelligent and Cognitive Systems Lab (LASIC)  
    Department of Exact Sciences  
    State University of Feira de Santana (UEFS)  

### URL: 
    http://sites.ecomp.uefs.br/lasic/projetos/libras-dataset  

### Date of Collection:
    October 9th, 2020

### License:
    Disclaimer "The dataset is free to use for scientific research."  

### Brief Description:  
    Dataset of hand gestures representing the Brazilian Sign Language (Libras). The dataset has 40 unique labels.
    For further information, please refer to the original source.

### Reference:  
    @inproceedings{dsLibras2015,
        author          = {I. L. O. {Bastos} and M. F. {Angelo} and A. C. {Loula}},
        booktitle       = {28th SIBGRAPI},
        title           = {Recognition of Static Gestures Applied to Brazilian Sign Language (Libras)},
        year            = {2015},
        doi             = {10.1109/SIBGRAPI.2015.26}
    }
 ---
---
## Dataset *ds-Food5k*  

### Source:  
    Multimedia Signal Processing Group  
    Ecole Polytechnique Fédérale de Lausanne  

### URL: 
    https://www.epfl.ch/labs/mmspg/downloads/food-image-datasets/  
    https://www.kaggle.com/binhminhs10/food5k  

### Date of Collection:
    October 1st, 2021

### License:
    Disclaimer:
    "" Permission is hereby granted, without written agreement and without license or royalty fees, to use, copy, modify, and distribute the data provided and its documentation for research purpose only. The data provided may not be commercially distributed. In no event shall the Ecole Polytechnique Fédérale de Lausanne (EPFL) be liable to any party for direct, indirect, special, incidental, or consequential damages arising out of the use of the data and its documentation. The Ecole Polytechnique Fédérale de Lausanne (EPFL) specifically disclaims any warranties. The data provided hereunder is on an “as is” basis and the Ecole Polytechnique Fédérale de Lausanne (EPFL) has no obligation to provide maintenance, support, updates, enhancements, or modifications. ""

### Brief Description:  
    Dataset of images depicting Food (2,500) and Non-Food (2,500).  

### Reference:  
    @inproceedings{dsFood2016,
        author        = {Singla, Ashutosh and Yuan, Lin and Ebrahimi, Touradj},  
        title         = {Food/Non-Food Image Classification and Food Categorization Using Pre-Trained GoogLeNet Model},  
        year          = {2016},
        isbn          = {9781450345200},
        publisher     = {Association for Computing Machinery},
        address       = {New York, NY, USA},
        url           = {https://doi.org/10.1145/2986035.2986039},
        note          = {DOI: 10.1145/2986035.2986039},
        booktitle     = {Proceedings of the 2nd International Workshop on Multimedia Assisted Dietary Management},
        pages         = {3–11},
        numpages      = {9},
        location      = {Amsterdam, The Netherlands},
        series        = {MADiMa '16},
    }
 ---
---
## Dataset *ds-Flickr-FireSmoke*  

### Source:  
    University of São Paulo  
    Institute of Mathematics and Computer Science (USP-ICMC)  
    Database and Image Group (GBdI)  

### URL:  
    https://github.com/mtcazzolato/dsw2017  

### Date of Collection:
    October 9th, 2020

### License:  
    Creative Commons  

### Brief Description:  
    Images acquired from Flickr, using tags related to fire and smoke to filter the information. Every image has two labels: one in L={fire, not fire} and one in L={smoke, not smoke}.  
    For further information, please refer to the original source.

### Reference:  
    @inproceedings{dsFlikrFire2015,
        author          = {Marcos Vinicius Naves Bedo and Gustavo Blanco and Willian D. Oliveira and Mirela T. Cazzolato and Alceu Ferraz Costa and Jos{\'{e}} Fernando Rodrigues-Jr. and Agma J. M. Traina and Caetano {Traina Jr.}},
        editor          = {Slimane Hammoudi and Leszek A. Maciaszek and Ernest Teniente},
        title           = {Techniques for Effective and Efficient Fire Detection from Social Media Images},
        booktitle = {{ICEIS} 2015 - Proceedings of the 17th International Conference on Enterprise Information Systems, Volume 1, Barcelona, Spain, 27-30 April, 2015},
        pages           = {34--45},
        publisher       = {SciTePress},
        year            = {2015},
        doi             = {10.5220/0005341500340045},
    }
---
---
## Dataset *ds-Covid19*  

### Source:  
    University of Montreal  
    Fontbonne University  
    Heidelberg University  
    Stony Brook Medicine  
    University of Toronto  

### URL:  
    https://github.com/ieee8023/covid-chestxray-dataset  

### Date of Collection:
    October 9th, 2020

### License:  
    Apache 2.0, CC BY-NC-SA 4.0, CC BY 4.0 (specific for each available image)

### Brief Description:  
    Open dataset of Chest X-Rays and Computed Tomographies (CTs) taken from patients which are positive or suspected of COVID-19 or other viral and bacterial pneumonias.
    For further information, please refer to the original source.

### Reference:  
    @article{dsCovid2020,
        title           = {COVID-19 Image Data Collection: Prospective Predictions Are the Future},
        author = {Joseph Paul Cohen and Paul Morrison and Lan Dao and Karsten Roth and Tim Q Duong and Marzyeh Ghassemi},
        journal         = {CoRR},
        volume          = {abs/2006.11988},
        eprint          = {2006.11988},
        year            = {2020},
        url             = {https://arxiv.org/abs/2006.11988}
    }
---
---
## Dataset *ds-COIL100*  

### Source:  
    Center for Research on Intelligent Systems  
    Department of Computer Science  
    Columbia University.  
### URL:  
    https://www.kaggle.com/jessicali9530/coil100  

### Date of Collection:  
    October 9th, 2020  

### License:  
    Disclaimer "This dataset is intended for non-commercial research purposes only."  
    
### Brief Description:  
    COIL stands for Columbia Object Image Library, a dataset composed of 100 different objects, depicted at angles in a 360 rotation, at every 5 degrees.
    As result, there are 72 pictures of every object, resulting on 7,200 imagens.
    For further information, please refer to the original source.

### Reference:  
    @techreport{dsCOIL1001996,
        author          = {S. A. Nene and S. K. Nayar and H. Murase},
        title           = {Columbia Object Image Library (COIL-100)},
        url             = {https://www.kaggle.com/jessicali9530/coil100},
        address         = {Technical Report CUCS-006-96},
        note            = {Last accessed in October, 2020},
    }
---
---
## Dataset *ds-CUB-200-2011*  

### Source:  
    University of California, San Diego  
    California Institute of Technology  

### URL: 
    http://www.vision.caltech.edu/visipedia/CUB-200-2011.html  

### Date of Collection:
    October 1st, 2021

### License:
    Not provided. Available under citation request.  

### Brief Description:  
    Images of 200 bird species acquired from Flickr, where each species is associated with a Wikipedia article and organized by a scientific classification among order, family, genus, and species.  

### Reference:  
    @techreport{dsCUB2011,
        title           = {The Caltech-UCSD Birds-200-2011 Dataset},
        author          = {Wah, C. and Branson, S. and Welinder, P. and Perona, P. and Belongie, S.},
        year            = {2011},
        institution     = {California Institute of Technology},
        number          = {CNS-TR-2011-001},
    }
 ---
---
## Dataset *ds-Letters*

### Source:  
    Created by Srdjan Hajder, aiming at recognizing the font type.  

### URL:  
    https://www.kaggle.com/killen/bw-font-typefaces/  

### Date of Collection:  
    October 9th, 2020  

### License:  
    CC BY-NC-SA 4.0  

### Brief Description:  
    Standard Windows fonts with each letters organized in classes by typeface.
    The labels of the dataset consists of 152 different typefaces.
    Alternativelly, users can analyze the dataset according to the different letters from each typeface.  
    For further information, please refer to the original source.  

### Reference:  
    @manual{dsLetters2020,
        title           = {Letters organized by typefaces},
        author          = {Srdjan Hajder},
        url             = {https://www.kaggle.com/killen/bw-font-typefaces?select=BRLNSR},
        year            = {2020},
        note            = {Last accessed in October, 2020},
    }
---
---
## Dataset *ds-Cars*  

### Source:  
    Computer Science Department  
    Stanford University  

### URL:  
    https://ai.stanford.edu/~jkrause/cars/car_dataset.html  

### Date of Collection:  
    October 9th, 2020

### License:  
    Disclaimer "This dataset is for research purposes only, similar to the ImageNet license (https://image-net.org/download.php)."

### Brief Description:  
    Images of cars from 196 classes, including MBR annotations. The dataset is divided into test and train.  
    For further information and label details, please refer to the original source.  

### Reference:  
    @inproceedings{dsCarsStanford2013,
        author          = {Jonathan Krause and Michael Stark and Jia Deng and Li Fei{-}Fei},
        title           = {3D Object Representations for Fine-Grained Categorization},
        booktitle       = {2013 {IEEE} International Conference on Computer Vision Workshops, {ICCV} Workshops 2013, Sydney, Australia, December 1-8, 2013},
        pages           = {554--561},
        publisher       = {{IEEE} Computer Society},
        year            = {2013},
        doi             = {10.1109/ICCVW.2013.77},
    }
---
---
## Dataset *ds-Food-11*  

### Source:  
    Multimedia Signal Processing Group  
    Ecole Polytechnique Fédérale de Lausanne  

### URL: 
    https://www.epfl.ch/labs/mmspg/downloads/food-image-datasets/  
    https://www.kaggle.com/binhminhs10/food5k  

### Date of Collection:
    October 1st, 2021

### License:
    Disclaimer:
    "" Permission is hereby granted, without written agreement and without license or royalty fees, to use, copy, modify, and distribute the data provided and its documentation for research purpose only. The data provided may not be commercially distributed. In no event shall the Ecole Polytechnique Fédérale de Lausanne (EPFL) be liable to any party for direct, indirect, special, incidental, or consequential damages arising out of the use of the data and its documentation. The Ecole Polytechnique Fédérale de Lausanne (EPFL) specifically disclaims any warranties. The data provided hereunder is on an “as is” basis and the Ecole Polytechnique Fédérale de Lausanne (EPFL) has no obligation to provide maintenance, support, updates, enhancements, or modifications. ""

### Brief Description:  
    Dataset of images depicting food, divided into 11 categories.  

### Reference:  
    @inproceedings{dsFood2016,
        author        = {Singla, Ashutosh and Yuan, Lin and Ebrahimi, Touradj},  
        title         = {Food/Non-Food Image Classification and Food Categorization Using Pre-Trained GoogLeNet Model},  
        year          = {2016},
        isbn          = {9781450345200},
        publisher     = {Association for Computing Machinery},
        address       = {New York, NY, USA},
        url           = {https://doi.org/10.1145/2986035.2986039},
        note          = {DOI: 10.1145/2986035.2986039},
        booktitle     = {Proceedings of the 2nd International Workshop on Multimedia Assisted Dietary Management},
        pages         = {3–11},
        numpages      = {9},
        location      = {Amsterdam, The Netherlands},
        series        = {MADiMa '16},
    }
 ---
---
## Dataset *ds-Dogs*

### Source:  
    Computer Science Department  
    Stanford University  

### URL:  
    http://vision.stanford.edu/aditya86/ImageNetDogs/  

### Date of Collection:  
    October 9th, 2020

### License:  
    Not specified. Only citation requirement.  

### Brief Description:  
    Images of dogs of 120 breeds from around the world. The dataset has 120 classes, one for each breed.
    For further information, please refer to the original source.  

### Reference:  
    @inproceedings{dsDogsStanford2011,
        author          = {Aditya Khosla and Nityananda Jayadevaprakash and Bangpeng Yao and Li Fei-Fei},
        title           = {Novel Dataset for Fine-Grained Image Categorization},
        booktitle       = {First Workshop on Fine-Grained Visual Categorization, IEEE Conference on Computer Vision and Pattern Recognition},
        year            = {2011},
        month           = {June},
        address         = {Colorado Springs, CO},
    }
---
---
## Dataset *ds-DeepLesion*  

### Source:  
    Department of Radiology and Imaging Sciences  
    National Institutes of Health Clinical Center  

### URL:  
    https://www.kaggle.com/kmader/nih-deeplesion-subset  
    https://nihcc.app.box.com/v/DeepLesion/  

### Date of collection:  
    October 7th, 2020  

### License:  
    Not provided. Available under citation request.  

### Brief Description:  
    Dataset with 32,120 slices extracted from 10,594 Computed Tomographies (CTs). Every CT is a study. The images were taken from 4,427 unique patients.   
    For further information, please refer to the original source.

### Reference:  
    @article{dsDeepLesion2017,
        author          = {Ke Yan and Xiaosong Wang and Le Lu and Ronald M. Summers},
        title           = {DeepLesion: Automated Deep Mining, Categorization and Detection of Significant Radiology Image Findings using Large-Scale Clinical Lesion Annotations},
        journal         = {CoRR},
        volume          = {abs/1710.01766},
        year            = {2017},
        url             = {http://arxiv.org/abs/1710.01766},
        archivePrefix   = {arXiv},
        eprint          = {1710.01766},
    }
---
---
## Dataset *ds-AwA*  

### Source:  
    Max Planck Institute for Informatics, Germany  
    IST (Institute of Science and Technology), Austria  
    University of Amsterdam, Netherlands  

### URL: 
    https://cvml.ist.ac.at/AwA2/  

### Date of Collection:
    October 1st, 2021

### License:
    Not provided. Available under citation request.  

### Brief Description:  
    Dataset with 37,322 images of animals divided into 50 classes.  

### Reference:  
    @article{dsAwa2019,
        author          = {Yongqin Xian and Christoph H. Lampert and Bernt Schiele and Zeynep Akata},
        title           = {Zero-Shot Learning - {A} Comprehensive Evaluation of the Good, the Bad and the Ugly},
        journal         = {{IEEE} Trans. Pattern Anal. Mach. Intell.},
        volume          = {41},
        number          = {9},
        pages           = {2251--2265},
        year            = {2019},
        url             = {https://doi.org/10.1109/TPAMI.2018.2857768},
        note            = {DOI: 10.1109/TPAMI.2018.2857768},
    }
 ---
--- 
## Dataset *ds-MNIST*  

### Source:  
    Yann LeCun from the Courant Institute of Mathematical Sciences  
    New York University  
    and  
    Corinna Cortes from Google Labs  
    
### URL:  
    http://yann.lecun.com/exdb/mnist/  

### Date of Collection:  
    October 9th, 2020  

### License:  
    Not provided.

### Brief Description:  
    Images of 10 handwritten digits (0 to 9). The date is divided into 60,000 training examples, and 10,000 test examples.  
    For further information, please refer to the original source.

### Reference:  
    @article{dsMNIST1998,
        author          = {Y. {Lecun} and L. {Bottou} and Y. {Bengio} and P. {Haffner}},
        journal         = {Proceedings of the IEEE}, 
        title           = {Gradient-based learning applied to document recognition}, 
        year            = {1998},
        volume          = {86},
        number          = {11},
        pages           = {2278-2324},
        }
---
---
## Dataset ds-*CompCars*  

### Source:  
    Department of Information Engineering  
    The Chinese University of Hong Kong  

    Shenzhen Key Lab of CVPR  
    Shenzhen Institutes of Advanced Technology  

    Chinese Academy of Sciences  

### URL:  
    http://mmlab.ie.cuhk.edu.hk/datasets/comp_cars/index.html  

### Date of Collection:  
    October 7th, 2020

### License:  
    Disclaimer:  
    ""  1. The CompCars database is available for non-commercial research purposes only.
        2. All images of the CompCars database are obtained from the Internet which are not property of MMLAB, The Chinese 3. University of Hong Kong. The MMLAB is not responsible for the content nor the meaning of these images.
        3. You agree not to reproduce, duplicate, copy, sell, trade, resell or exploit for any commercial purposes, any portion of the images and any portion of derived data.
        4. You agree not to further copy, publish or distribute any portion of the CompCars database. Except, for internal use at a single site within the same organization it is allowed to make copies of the database.
        5. The MMLAB reserves the right to terminate your access to the database at any time.
        6. All submitted papers or any publicly available text using the CompCars database must cite the following paper:
            Linjie Yang, Ping Luo, Chen Change Loy, Xiaoou Tang. A Large-Scale Car Dataset for Fine-Grained Categorization and Verification, In Computer Vision and Pattern Recognition (CVPR), 2015. ""
    
### Brief Description:  
    Images depicting cars, taken from two scenarios: web-nature with 136,726 car images and 27,618 images of car parts; and surveillance-nature with 50,000 cars (front vire).  
    For further information, please refer to the original source.  

### Reference:  
    @inproceedings{dsCars2015,
        author          = {Linjie Yang and Ping Luo and Chen Change Loy and Xiaoou Tang},
        title           = {A large-scale car dataset for fine-grained categorization and verification},
        booktitle       = {{IEEE} Conference on Computer Vision and Pattern Recognition, {CVPR} 2015, Boston, MA, USA, June 7-12, 2015},
        pages           = {3973--3981},
        publisher       = {{IEEE} Computer Society},
        year            = {2015},
        doi             = {10.1109/CVPR.2015.7299023},
    }
