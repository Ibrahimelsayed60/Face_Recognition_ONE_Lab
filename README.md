# Face Recognition

Facial recognition is the task of making a positive identification of a face in a photo or video image against a pre-existing database of faces. It begins with detection - distinguishing human faces from other objects in the image - and then works on identification of those detected faces.

One of the simplest and most effective PCA approaches used in face recognition systems is the so-called eigenface approach. This approach transforms faces into a small set of essential characteristics, eigenfaces, which are the main components of the initial set of learning images (training set). Recognition is done by projecting a new image in the eigenface subspace, after which the person is classified by comparing its position in eigenface space with the position of known individuals . The advantage of this approach over other face recognition systems is in its simplicity, speed and insensitivity to small or gradual changes on the face. The problem is limited to files that can be used to recognize the face.

## Dataset

Link of dataset:https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/

Choose faces only data (1GB).

Pre-Processed data link: https://drive.google.com/file/d/1f7uzliQb-9KhC4TOLIb-wSFqk5flxpx-/view?usp=sharing

## Process

The whole recognition process involves two steps:

1. **Initialization process**
2. **Recognition process**

The Initialization process involves the following operations: 

​	i. Acquire the initial set of face images called as training set. 

​	ii. Calculate the Eigenfaces from the training set, keeping only the highest eigenvalues. These 	M images define the face space. As new faces are experienced, the eigenfaces can be     		           updated or recalculated. 

​	iii. Calculate distribution in this M-dimensional space for each known person by projecting  		his or her face images onto this face-space.

<img src="Images\photo1.png" alt="photo1" style="zoom:80%;" /><img src="Images\photo2.png" alt="photo2" style="zoom:100%;" />