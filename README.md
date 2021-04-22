# Cilia Segmentation
## Team - Tamiyo
This project is implemented as a part of the Data Science Practicum (CSCI 8360) course at the University of Georgia. The goal was to develop a video segmentation pipeline that identifies the regions of the videos containing cilia as accurately as possible. Cilia are microscopic hairlike structures that protrude from literally every cell in your body. They beat in regular, rhythmic patterns to perform myriad tasks, from moving nutrients in to moving irritants out to   amplifying cell-cell signaling pathways to generating calcium fluid flow in early cell differentiation.

## Dataset:
The data are all available on GCP: gs://uga-dsp/project3<br> 
In that parent folder, there are two subfolders: data and masks. 
<ul>
  <li>Data contains a bunch of folders (325 of them), named as hashes, each of which contains 100 consecutive frames of a grayscale video of cilia.</li>
  <li>Masks contain a number of PNG images (211 of them), named as hashes (corresponding to the subfolders of data), 
      that identify regions of the corresponding videos where cilia is. </li>
  <li>Also within the parent folder are two text files: train.txt and test.txt </li>
 
</ul>
 

## Installation
* [Google Cloud Platform](https://cloud.google.com/)
* [Tensorflow](https://www.tensorflow.org/install)
* [Python 3.6+](https://www.python.org/)
* [Jupyter Notebook](https://jupyter.org/install) is a popular application that enables you to edit, run and share Python code into a web view. It allows you to modify and re-execute parts of your code in a very flexible way. 

## Contributions
Please see [CONTRIBUTORS](https://github.com/dsp-uga/tamiyo-p3/blob/main/CONTRIBUTORS.md) file for more details.

## Authors 
(Ordered alphabatically)
<ul> 
  <li><a href= "https://github.com/mashihan123"> Shihan Ma</a></li>
  <li><a href ="https://github.com/shivamchandan93" > Shivam Chandan </a></li>
  <li><a href = "https://github.com/shophine"> Shophine Sivaraja</a></li>
</ul>

## License
This project is licensed under the MIT License - see the <a href="https://github.com/dsp-uga/tamiyo-p3/blob/main/LICENSE">LICENSE</a> file for the details.

## Approach
* U-Net
  * It is a Convolution Neural Networks for Biomedical Image Segmentation
  * Best architecture to work with less training samples(images) 
  

## References
* [U-Net Model](https://github.com/bnsreenu/python_for_microscopists/blob/master/204-207simple_unet_model.py)
* [PyTorch](https://pytorch.org/tutorials/intermediate/torchvision_tutorial.html) - RCNN with Pytorch
* [Semantic Segmentation](https://medium.com/@pallawi.ds/semantic-segmentation-with-u-net-train-and-test-on-your-custom-data-in-keras-39e4f972ec89)
