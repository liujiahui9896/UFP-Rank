# UFP-Rank

These are the dataset used in UFP-Rank.
## Citation:
Please cite this paper if you refer to the related information.

    User-Aware Folk Popularity Rank: User-Popularity-Based Tag Recommendation That Can Enhance Social Popularity
    Xueting Wang, Yiwei Zhang, Toshihiko Yamasaki (The University of Tokyo)
    ACM Multimedia 2019



## Training:
### Description: 
    The source dataset is used to train the adjacency matrix of tags.
    We randomly select 60,000 images (uploaded by 6462 users) with over 20 tags and over 5000 views from Flickr’s public data set YFCC100M (http://projects.dfki.uni-kl.de/yfcc100m/).
    The id number of selected images and corresponding users are shown in the File train_flickr_id.csv.

    You can get other information including images, views, tags from the page of YFCC100M or through the Flickr API (https://www.flickr.com/services/api/). 
    Note that some images are not avalible on Flickr now.

### Format:
    image_id, user_id

## Testing:
### Description:
    We created a target dataset for testing to conduct the tag recommendation and uploading experiment to verify the popularity enhancing performance.
    We randomly selected 1000 images (only 990 images were succussfully uploaded to Flickr during experiments) from Wikimedia Commons (https://commons.wikimedia.org/wiki/Main_Page).
    The id number of selected images are shown in the File test_wiki_id.csv.

    The corresponding initial tags were generated according to the image contents automatically by a computer vision API provided by the Microsoft Cognitive Services (https://azure.microsoft.com/en-us/services/cognitive-services/computer-vision/).

### Format:
    image_id
