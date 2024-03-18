# CCTV Action Recogintion System for Stores

This project focuses on recognizing actions in videos, particularly targeting shoplifting detection in surveillance footage. We utilize an advanced neural network architecture known as Inception I3D (Inception-3D) for this purpose. The Inception I3D model is a state-of-the-art deep learning architecture specifically designed for action recognition tasks in videos. It combines the power of both spatial and temporal features through its intricate design, making it highly effective in capturing complex motion patterns.

### Methodology

- **Data Preparation**: The dataset consists of video clips categorized into different actions, primarily focusing on normal behavior and shoplifting instances.
- **Data Augmentation**: We generate frames from the video clips, ensuring a consistent number of frames per video to maintain uniformity across the dataset. Random oversampling is applied to balance the class distribution in the training set.
- **Model Architecture**: The Inception I3D model architecture is employed, featuring convolutional and pooling layers along with inception modules that capture spatial and temporal features effectively.
- **Training**: The model is trained on the training dataset with class weights to handle class imbalance, optimizing towards minimizing cross-entropy loss and maximizing accuracy.
- **Evaluation**: The trained model is evaluated on both validation and test datasets to assess its generalization performance.
- **Prediction and Inference**: The model is used to predict actions in video clips, particularly focusing on shoplifting detection in surveillance footage.

### Conclusion

This project showcases the development of a CCTV Action Recognition System for stores, focusing on the critical task of detecting shoplifting incidents in surveillance footage. By employing the sophisticated Inception I3D model, we have achieved significant progress in accurately identifying and classifying actions within video data.

### Key Metrics and Model Details

- **Model Architecture**: Inception I3D
- **Number of Parameters**: Approximately 3 million
- **Accuracy**: Achieved approximately 91.7% accuracy on the test dataset
- **Precision and Recall**:
  - Precision for normal behavior: Approximately 88.2%
  - Precision for shoplifting detection: 100%
  - Recall for normal behavior: 100%
  - Recall for shoplifting detection: Approximately 77.8%

### Future Prospects and Use Cases

Moving forward, this system holds immense potential for various applications and advancements:

- **Real-time Deployment**: Deployment in real-time surveillance systems can enable proactive detection and prevention of shoplifting incidents, enhancing store security.
- **Integration with Security Systems**: Integration into existing security infrastructure can bolster surveillance networks, ensuring better protection of assets and public safety.
- **Transfer Learning**: The trained model can be leveraged for transfer learning in related tasks, extending its utility beyond shoplifting detection to general action recognition in diverse domains.
- **Continuous Improvement**: Continuous refinement and updates based on real-world data can further enhance the system's accuracy and effectiveness, ensuring its relevance and reliability over time.

This project demonstrates the potential of advanced deep learning techniques in enhancing security measures and public safety through intelligent video analytics. The ability to recognize complex actions in real-time opens up numerous opportunities for developing proactive surveillance systems that can effectively mitigate security threats and protect public and private assets.