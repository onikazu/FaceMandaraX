# FaceMandara
## abstract
FaceMandara searches similar face from over 200,000 face data(celebA) to you in real time.


## dependency
dlib
face_recognition
faiss

~~~
faiss
# CPU version only
conda install faiss-cpu -c pytorch
# Make sure you have CUDA installed before installing faiss-gpu, otherwise it falls back to CPU version
conda install faiss-gpu -c pytorch # [DEFAULT]For CUDA8.0
conda install faiss-gpu cuda90 -c pytorch # For CUDA9.0
conda install faiss-gpu cuda91 -c pytorch # For CUDA9.1
# cuda90/cuda91 shown above is a feature, it doesn't install CUDA for you.
~~~

## Usage
- At first, install the packages

```Tarminal
$ pip install -r requirements.txt
```
- install faiss which is the package which do PV
```
# CPU version only
$ conda install faiss-cpu -c pytorch
# Make sure you have CUDA installed before installing faiss-gpu, otherwise it falls back to CPU version
$ conda install faiss-gpu -c pytorch # [DEFAULT]For CUDA8.0
$ conda install faiss-gpu cuda90 -c pytorch # For CUDA9.0
$ conda install faiss-gpu cuda91 -c pytorch # For CUDA9.1
# cuda90/cuda91 shown above is a feature, it doesn't install CUDA for you.
```

- download CelebA dataset and put the data to "big_database_def" directory.
[CelebA dataset](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)

- Rename the directory "big_database_def" to "big_database"

- Then put the command terminal like bellow

```Tarminal
$ python face_mandara.py
```
