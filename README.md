# forest-aerial-segmentation-with-Unet
# Forest Enumeration Using Aerial Segmentation for Environmental Impact Reduction

### Overview
This project aims to aid environmental conservation efforts by detecting and segmenting forested areas in aerial imagery, helping monitor deforestation impacts from coal mining and other industrial activities. Using a U-Net model for semantic segmentation, the project identifies forest regions and contributes to resource management for sustainability.

### Motivation
This project was inspired by a problem statement from the Smart India Hackathon, which sought solutions to reduce deforestation caused by mining activities. Although there was no exact match, the project adapts the challenge by focusing on forest segmentation using aerial imagery, providing a base for forest resource monitoring and impact assessment.

### Dataset
- **Source**: [Kaggle - Forest Segmentation Dataset](https://www.kaggle.com/datasets/quadeer15sh/augmented-forest-segmentation)
- The dataset contains labeled aerial images for training and testing.
- **Instructions**: Download the dataset from Kaggle using the link above. Follow the data loading instructions in the notebook to prepare the data for training and evaluation.

### Model and Methodology
The **U-Net architecture** was chosen for its effectiveness in image segmentation tasks, particularly for capturing fine-grained details. Key elements of the methodology include:
- **Preprocessing**: Images and masks are resized to a standard size, normalized, and augmented to improve model robustness.
- **Architecture**: U-Net is implemented with encoder and decoder blocks, optimizing for pixel-level accuracy in detecting forest regions.
- **Training**: Binary cross-entropy is used as the loss function, with additional metrics like Dice Coefficient and Mean Intersection over Union (Mean IoU) to evaluate model performance.

### Results
The following images demonstrate segmentation results, including comparisons between true and predicted masks:

#### Example Results
![True Mask vs Predicted Mask 1]![Screenshot 2024-11-04 084157](https://github.com/user-attachments/assets/6cbc0b70-e5e5-4c06-8124-9a3ffe4b9411)

![True Mask vs Predicted Mask 2]![Screenshot 2024-11-04 084209](https://github.com/user-attachments/assets/ac9f172b-9b02-4dea-b362-77406607931c)

![True Mask vs Predicted Mask 3]![Screenshot 2024-11-04 084222](https://github.com/user-attachments/assets/d27c30c0-e180-4c20-a9d2-e0a3a0e2e41a)


### Future Work
This project is in its initial stages, with plans for further development:
- **Deployment**: Exploring deployment as a web app or REST API for real-time forest monitoring.
- **Data Quality Enhancements**: Improving label consistency in the dataset to enhance model performance.
- **Alternate Architectures**: Testing other segmentation models to potentially improve accuracy.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/AnuragNegi21/forest-enumeration-segmentation.git
