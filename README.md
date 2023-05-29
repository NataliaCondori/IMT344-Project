# Bolivian Signal Detection (BSD)
The project is Sign language detection from finger and face trajectory. For this it was necessary to create a dataset consisting of videos of 20 different signs, from this dataset we proceeded with the pre-processing part to normalize the number of frames and the size of the videos.  Mediapipe was then used to record the trajectories of the hand and parts of the face such as the eyes. Finally, a model was applied for data training, evaluation and testing.

## Motivation
This project took as a reference a problem present in society: social inclusion. We consider that a group of people who often lack opportunities are those with hearing disabilities, in that sense we wanted to support inclusion through this model that allows to recognize sign language automatically, in this way we achieve a support for a more effective communication.

## Screenshots

![Video first](Preview3.png)
![Video first](Preview1.png)
![Video first](Preview2.png)
![Video first](Preview6.png)
![Video first](Preview5.png)
![Video first](Preview4.png)


## Tecnologies
- Mediapipe
- Tensorflow 
- Google Drive
- Google Colab

## Important functionalities
Undoubtedly the most interesting functionality of the project is the method of using Mediapipe for optimal recognition based on the trajectories of the different parts of the hand and face. For the fingers, we use different colors, since the trajectory of each finger has a lot of weight for the prediction of the signs, additionally the use of Mediapipe in the face, such as the eyes, is due to the fact that many signs are similar but the fact of having referenced the face, provides a necessary support for a correct detection.

## Instalation
- The first step is to have stored the videos that will be part of the dataset, it is essential that the files are stored in individual folders that will be referenced by the type of signal.
- Then it is necessary to open the normalize.ipynb file that allows to establish a similar ratio of frames for all the videos in the dataset, the number of frames can be adjusted according to the application, these videos will be saved in the dataset folders so the original videos can be deleted.
- Then the next step is to open the Mediapipe_detection.ipynb file that will allow to take as input the normalized videos from the previous stage, then the code applies the use of Mediapipe to find the essential points and plots them in one image per video, these images are stored for the last stage of the model.
- Finally, the .ipynb file allows to generate a training, testing and evaluation set from the images generated with Mediapipe by mixing all the images from all of them. Note: the lines of code are commented in order to provide the necessary information for the necessary changes.

## Credits
List of participants for this project:
- Ever Imanol Alavi Gallardo
- Natalia Lourdes Condori Peredo
- Weimar Adalid Condori Yupanqui
- Carlos Mauricio Fernadez Aldayuz
- Diego Alfredo Rodríguez Martinez

## License

The MIT License

Copyright (c) 2023 [NDEAH]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
