# 2018 ISIC Challenge (Task 3) Reader Study data
The data in this folder refer to two collections. Reads in files marked as
``training`` belong to the training set collection (10,015 images). Reads in
files marked as ``test`` belong to the test set collection (1,512 images):

- [2018 Challenge Task 3 training set collection](https://api.isic-archive.com/collections/66/)
- [2018 Challenge Task 3 test set collection](https://api.isic-archive.com/collections/67/) (login required!)

## Study design
Readers were shown either images from the training or test set collections
one by one in batches of 30 images. For each image, readers were asked to
make a diagnosis guess among the following options:

- actinic keratoses or intra-epithelial carcinoma (label: AKIEC)
- basal cell carcinoma (label: BCC)
- benign keratosis (solar lentigine/seborrheic keratoses or lichen-planus like keratosis, label: BKL)
- dermatofibroma (label: DF)
- melanoma (label: MEL)
- nevus (label: NV)
- vascular lesions (angiomas, angiokeratomas, pyogenic granulomas and hemorrhages, label: VASC)

## CSV files
The following files are available for this set of images:

- ``training_set_isic.csv`` - aggregated responses across all readers
- ``training_set_isic_derms.csv`` - aggregated responses across dermatologists
- ``training_set_isic_exp.csv`` - aggregated responses across experts
- ``training_set_isic_nonexp.csv`` - aggregated responses across non-experts
- ``test_set_isic.csv`` - aggregated responses across all readers
- ``test_set_isic_derms.csv`` - aggregated responses across dermatologists (does not cover all images!)
- ``test_set_isic_exp.csv`` - aggregated responses across experts (does not cover all images!)
- ``test_set_isic_nonexp.csv`` - aggregated responses across non-experts

## CSV file contents
Each row of the CSV files specifies the image ID the reads relate to,
together with the raw counts for each of the reader-chosen diagnoses,
as well as the ground-truth for that respective image.

