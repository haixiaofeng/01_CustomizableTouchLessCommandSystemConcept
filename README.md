</br>

### bindOI: Operation Interface Concept For the Visually Impaired
</br>
</br>

#### Code & Files
- [Code folder](https://drive.google.com/drive/folders/1yUbV3VjX3Jasnvd_OFGMxiV0u8tXPYp6?usp=sharing)
- [Data foler](https://drive.google.com/drive/folders/1dTroHtgS9cep5CFhvXOFp-z-8uQaxCka?usp=sharing)
- [Model folder](https://drive.google.com/drive/folders/1iO76YteRA0e2U6wuBDHDtrucM66aWJhu?usp=sharing)
</br>
</br>

#### Motivation
Computers that require operation through direct touch with the devices create an extra layer of inconvenience for the visually impaired. Developing a concept for a more user-friendly Operation Interface (OI) leverging existing computer vision technologies without the need for direct mannual controls yeilds a better use case for these population. Such an OI may also be extended to more advanced use cases as the world moves into the era of VR/AR. 
</br>
</br>

#### Data
Data are collected as coordinates of landmarks over face, left hand, right hand, and pose using MediaPipe extracted from webcam captures with CV2. Specifically, landmarks from 30 webcam captures (videos) each 30 frames long are saved for each command (there are 3 currently supported commands) for training. There are a total of 1,662 landmarks in each captured frame. Refer to [this]() short recording of the data collection process.
</br>
</br>

#### Algorithm
A Long/Short-Term Memory (LSTM) Neural Network is used for training. Please refer to the code file for details
</br>
</br>

#### Current Results
The current test accuray is very close to 1 but is less robust in a practical sense as it handels transitions between commands less well (i.e. confusion or slow recognition between commands)
</br>
</br>
</br>

--

</br>

#### Version History
- Version 1: Minimum working pipeline (utilities, data collection, modeling, training, evaluation, and live demo) with demonstrable but suboptimal performance

#### Future Versions
- Version 2: Collect more variations of training data to incorporate more shapes & sizes of bodies and hands to improve action recognition accuracy
- Version 3: Further refine training data and model to improve action recognition _efficiency_ (i.e. how long it takes to make an accurate prediction)
- Version 4: Include more commands
