# SCUT_FORU_DB_Release

# SCUT-FORU: Flickr OCR Universal Database

Flickr OCR Universal Database (abbreviated as FORU and pronounced like for you) is collected from Flickr website https://www.flickr.com/ and now released by Human Computer Intelligent Interaction Lab of South China University of Technology. The database can be downloaded by https://www.dropbox.com/s/06wfn5ugt5v3djs/SCUT_FORU_DB_Release.rar?dl=0. or https://pan.baidu.com/s/1bprajkN


## 1 Database Organization

FORU contains two parts, which are Chinese2k and English2k dataset, respectively.


### (a) English2k dataset

English2k dataset is consists of two subsets, which one subset is suitable for character detection and the other one is suitable for word detection. The character detection subset has 813 training images and 349 testing images. The detailed annotations are presented in Table 1. On the other hand, the word detection subset has 1200 training images and 515 testing images. The detailed annotations are presented in Table 2.

Table 1 Character Level Bounding boxes

| name | Training Bounding box Instances | Testing Bounding box Instances | Total Bounding box Instances |
| ---------- | ---------- | ---------- | ---------- |
| English2k |  14888 | 6506 | 21394 |

Table 2 Word Level Bounding boxes

| name | Training Bounding box Instances | Testing Bounding box Instances | Total Bounding box Instances |
| ---------- | ---------- | ---------- | ---------- |
| English2k |  3840 | 1581 | 5421 |

### (b) Chinese2k dataset

The Chinese2k dataset has 1861 training images and 355 testing images. The detailed annotation is presented in Table 3.

 Table 3 Annotations of Chinese2k dataset

| name | Training Bounding box Instances | Testing Bounding box Instances | Total Bounding box Instances |
| ---------- | ---------- | ---------- | ---------- |
| Chinese2k |  23768 | 4626 | 28394 |

## 2 Format of ground truth files

Each image in the database corresponds to a ground truth file, in which each line records the location and label of one character/word. The format of the ground truth files is illustrated as {x, y, w, h, label}. {x, y} denotes the top-left coordinate of the annotated bounding box, and {w, h} denotes the size of the annotated bounding box.

## 3 Database Usage

The samples of SCUT-FORU dataset have a great diversity. The scenes include streets, buildings, shops, offices, restaurants, railway stations, subway, etc. The texts include traffic signs, road signs, book covers, outdoor advertising, signs, and so on. Various light conditions are also considered, such as sunny and cloudy, day and night, and so on. It is worth noting that most text directions are horizontal. This database should be used for scene text detection and recognition. Specifically, it is available in the field of 

(A) cropped character recognition; 

(B) cropped word recognition and 

(C) full image word detection and recognition.

## 4 Contact

Please consider to cite our paper 
```
@inproceedings{zhang2016character,
  title={Character proposal network for robust text extraction},
  author={Zhang, Shuye and Lin, Mude and Chen, Tianshui and Jin, Lianwen and Lin, Liang},
  booktitle={Acoustics, Speech and Signal Processing (ICASSP), 2016 IEEE International Conference on},
  pages={2633--2637},
  year={2016},
  organization={IEEE}
}
```
when you use our database. Please feel free to modify the dataset when it is needed. For any questions about this database please contact shuye.cheung@gmail.com or lianwen.jin@gmail.com.
