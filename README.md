# Malaria Detection in Blood Samples

## Overview

This project is an image processing-based system for the automatic detection of malaria parasites from microscopic blood smear images. It aims to reduce human error, speed up diagnosis, and assist healthcare professionals in identifying infected red blood cells (RBCs).

## Problem Statement

Traditional malaria diagnosis is performed manually by examining stained blood smear slides under a microscope. This process is:
- Time-consuming
- Dependent on expert pathologists
- Prone to human error

This project automates the detection process using image processing techniques.

## Features

- Load blood smear images
- Extract Red Blood Cells (RBCs)
- Count total RBCs
- Detect malaria parasites
- Count infected cells
- Calculate infection ratio
- Automatic image segmentation and analysis

## System Architecture

```
Input Image
     │
     ▼
Color Analysis
     │
     ▼
Image Segmentation
     │
     ▼
Feature Extraction
     │
     ▼
Classification
     │
     ▼
Detection Results
```

## Algorithm Workflow

1. Load digital RGB blood smear image
2. Extract Red Blood Cells (RBCs)
3. Count total RBCs
4. Detect malaria parasites
5. Count parasites
6. Calculate infected vs. uninfected RBC ratio

## Image Processing Techniques

### RBC Extraction
- Color-based thresholding
- RGB color range filtering

### RBC Counting
- Convert image to grayscale
- Convert grayscale to binary
- Region-based analysis
- Count RBCs

### Image Segmentation
- Otsu's Thresholding
- Edge Detection (Canny)
- Morphological Operations
  - Dilation
  - Hole Filling

### Parasite Detection
- Color-based segmentation
- RGB thresholding
- Binary image conversion
- Region analysis for parasite counting

## Technologies Used

- Image Processing
- Digital Image Analysis
- RGB Color Segmentation
- Otsu Thresholding
- Canny Edge Detection
- Morphological Processing

## Applications

- Automated malaria diagnosis
- Medical image analysis
- Clinical decision support
- Faster laboratory diagnosis
- Areas with limited medical experts

## Results

| Total Cells | Detected | Efficiency |
|-------------|----------|------------|
| 843 | 744 | 88.25% |
| 338 | 273 | 80.76% |
| 1181 | 1017 | 86.11% |

Overall detection efficiency: **80–88%**

## Conclusion

This system automates malaria parasite detection from blood smear images using image processing techniques. It minimizes human error, speeds up diagnosis, and provides reliable results with high detection accuracy. Such systems can support pathologists and improve healthcare services, especially in regions with limited medical expertise.

## Future Improvements

- Integrate Deep Learning (CNN)
- Improve detection accuracy
- Real-time diagnosis
- Mobile application support
- Cloud-based analysis

## License

This project is intended for educational and research purposes.
Author Mudasir Ahmad // @ Anberlin
