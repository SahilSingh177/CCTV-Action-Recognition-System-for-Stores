# CCTV Action Recogintion System for Stores

This project focuses on recognizing actions in videos, particularly targeting shoplifting detection in surveillance footage. We utilize an advanced neural network architecture known as Inception I3D (Inception-3D) for this purpose. The Inception I3D model is a state-of-the-art deep learning architecture specifically designed for action recognition tasks in videos. It combines the power of both spatial and temporal features through its intricate design, making it highly effective in capturing complex motion patterns.

### Methodology

- **Data Preparation**: The dataset consists of video clips categorized into different actions, primarily focusing on normal behavior and shoplifting instances.
- **Data Augmentation**: We generate frames from the video clips, ensuring a consistent number of frames per video to maintain uniformity across the dataset. Random oversampling is applied to balance the class distribution in the training set.
- **Model Architecture**: The Inception I3D model architecture is employed, featuring convolutional and pooling layers along with inception modules that capture spatial and temporal features effectively.
- **Training**: The model is trained on the training dataset with class weights to handle class imbalance, optimizing towards minimizing cross-entropy loss and maximizing accuracy.
- **Evaluation**: The trained model is evaluated on both validation and test datasets to assess its generalization performance.
- **Prediction and Inference**: The model is used to predict actions in video clips, particularly focusing on shoplifting detection in surveillance footage.

### Key Metrics and Model Details
![model](https://github.com/SahilSingh177/CCTV-Action-Recognition-System-for-Stores/assets/96344003/45eb44a3-1cba-4f7d-b64e-cca77ff57c44)
![image](https://github.com/SahilSingh177/CCTV-Action-Recognition-System-for-Stores/assets/96344003/ec246326-96dd-458b-96f0-097ed826b308)

- **Model Architecture**: Inception I3D
- **Number of Parameters**: Approximately 3 million
- **Accuracy**: Achieved approximately 91.7% accuracy on the test dataset
- **Precision and Recall**:
  - Precision for normal behavior: Approximately 88.2%
  - Precision for shoplifting detection: 100%
  - Recall for normal behavior: 100%
  - Recall for shoplifting detection: Approximately 77.8%

### Data Source
The dataset utilized in this project is the UCF-Crime dataset, a widely used benchmark dataset for action recognition tasks in surveillance videos. However, to adapt it for the specific task of shoplifting detection, extensive preprocessing and cleaning were necessary.

### Data Preprocessing
Given the long duration of the videos in the UCF-Crime dataset, a significant preprocessing effort was undertaken to extract relevant segments containing instances of shoplifting. This involved segmenting the videos into shorter clips focused on the periods of interest, thereby ensuring that the dataset appropriately represents the target behavior.

### Conclusion
This project showcases the development of a CCTV Action Recognition System for stores, focusing on the critical task of detecting shoplifting incidents in surveillance footage. By employing the sophisticated Inception I3D model, we have achieved significant progress in accurately identifying and classifying actions within video data.

### References
- https://arxiv.org/abs/1705.07750 (Quo Vadis, Action Recognition? A New Model and the Kinetics Dataset)
- https://www.tensorflow.org/hub/tutorials/movinet
- https://paperswithcode.com/task/action-recognition-in-videos
  
### Future Prospects and Use Cases

Moving forward, this system holds immense potential for various applications and advancements:

- **Real-time Deployment**: Deployment in real-time surveillance systems can enable proactive detection and prevention of shoplifting incidents, enhancing store security.
- **Integration with Security Systems**: Integration into existing security infrastructure can bolster surveillance networks, ensuring better protection of assets and public safety.
- **Transfer Learning**: The trained model can be leveraged for transfer learning in related tasks, extending its utility beyond shoplifting detection to general action recognition in diverse domains.
- **Continuous Improvement**: Continuous refinement and updates based on real-world data can further enhance the system's accuracy and effectiveness, ensuring its relevance and reliability over time.

This project demonstrates the potential of advanced deep learning techniques in enhancing security measures and public safety through intelligent video analytics. The ability to recognize complex actions in real-time opens up numerous opportunities for developing proactive surveillance systems that can effectively mitigate security threats and protect public and private assets.
