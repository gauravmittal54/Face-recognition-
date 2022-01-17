# Face-recognition-
Face detection is one of the fundamental applications used in face recognition technology. Facebook, Amazon, Google and other tech companies have different implementations of it. Before they can recognize a face, their software must be able to detect it first. Amazon has developed a system of real time face detection and recognition using cameras. Facebook uses it mostly on photos that their users upload in order to suggest tagging friends.

In this project, I implemented a system for locating faces in digital images. These are in JPEG format only. Before we continue, we must differentiate between face recognition and face detection. They are not the same, but one depends on the other. In this case face recognition needs face detection for making an identification to “recognize” a face. I will only cover face detection.

Understanding Haar Cascades
A Haar Cascade is based on “Haar Wavelets” which Wikipedia defines as:
A sequence of rescaled “square-shaped” functions which together form a wavelet family or basis.

Feature Extraction
As I mentioned earlier, Haar Cascades use machine learning techniques in which a function is trained from a lot of positive and negative images. This process in the algorithm is feature extraction.

![image](https://user-images.githubusercontent.com/61792468/149770204-d14aab9a-4ff9-469b-ae57-67b45d57529e.png)

Running OpenCV
For this project I prepared a directory where I dumped all the files needed. You will need to put in this directory the following:
face_detection.py (the name I gave to the Python program that contains code. This name can be changed.)
haarcascade_frontalface_default.xml (Haar Cascade training data)
photos



Results
Test #1. Single Face

![img1](https://user-images.githubusercontent.com/61792468/149773598-d8deb0a2-2e28-44c1-8418-81622e3b62f4.jpg)


Test #2. Two Faces

![img4 (2 person in a frame)](https://user-images.githubusercontent.com/61792468/149773658-2060ba47-97c0-42fc-bfa4-2cbbd90ba883.jpg)


Test #3. Three Faces

![img3(3 person in a frame)](https://user-images.githubusercontent.com/61792468/149773692-d27afe64-2d87-42ec-8623-bac270141ea5.jpg)



Test #4. Four Faces

![img3](https://user-images.githubusercontent.com/61792468/149773746-368b9cc4-ac78-4dfc-9e36-b81fe6fe0ae1.jpg)

Test #7. Non-Human Faces

The first non-human face I tested was from the cat photo. Now I tried using various parameters, but the algorithm had failed to detect the face using the values I entered.

![cat img](https://user-images.githubusercontent.com/61792468/149774402-8d7b1051-816a-4928-a7c5-3c369e1b0503.jpg)

![monkey img](https://user-images.githubusercontent.com/61792468/149774553-5478a93c-e058-4b81-bdc2-08a89167389d.jpg)


Since the monkey is a member of the primate family to which humans belong, the similarities may be the reason why it would be more accurately detected. Certainly more tests can be done with non-human faces to see how it compares with the training data. A more appropriate way to detect animal faces is with a classifier trained using animal photos.




