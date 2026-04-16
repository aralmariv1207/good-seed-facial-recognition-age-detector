# Good Seed: Facial Recognition Age Detector

A computer vision solution for automated age estimation from images, utilizing Transfer Learning with the ResNet50 architecture and TensorFlow/Keras.

## 🚀 Technical Highlights

- **Transfer Learning Architecture:** Utilized a **ResNet50** backbone pre-trained on ImageNet, fine-tuned for the specialized task of human age estimation.
- **Deep Learning for Regression:** Adapted the final layer with a linear activation function to predict continuous age values (regression) rather than discrete classification categories.
- **Optimized Data Flow:** Leveraged TensorFlow's `ImageDataGenerator` and `flow_from_dataframe` to efficiently stream 7.6k images directly from disk, maintaining a low memory footprint during training.
- **Performance Metric:** Achieved a competitive **Mean Absolute Error (MAE)**, validating the model's ability to generalize across diverse facial features and lighting conditions.
- **Preprocessing Pipeline:** Implemented automated image rescaling and target-size normalization ($224 \times 224$) to ensure data consistency across the APPA-REAL dataset.
