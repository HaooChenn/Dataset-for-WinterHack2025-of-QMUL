# 🤖 Dataset-for-WinterHack2025-of-QMUL (Path Tracking Robot Vision Dataset)

## 📊 Dataset Overview
This dataset is specifically designed for autonomous path tracking robots' visual recognition tasks, comprising two meticulously collected subsets. The data was gathered for the Winter Hack 2025' event organized by Queen Mary University of London (QMUL), aiming to enhance robotic target recognition capabilities in real-world scenarios.

## 🎯 Dataset Details
### Bullseye Dataset
- Volume: 328 high-quality annotated samples
- Target class: Single class `bullseye`
- Application: Precise localization and target center recognition
- Characteristics: Contains bullseye images at various scales and angles

### 🦆 Rubber Duck Dataset
- Volume: 412 annotated samples
- Target class: Single class `duck`
- Application: Object recognition and tracking
- Characteristics: Features rubber duck images under varying poses and lighting conditions

## 📸 Data Collection Methodology
### Equipment and Environment
- Collection device: High-definition camera mounted on path tracking robot
- Capture environment: Controlled laboratory conditions
- Lighting setup: Professional lighting equipment for ensuring data diversity

### Collection Strategy
1. Each target object captured from a minimum of 80 distinct angles
2. Data augmentation through lighting intensity adjustment at each angle:
   - High illumination: Simulating intense daylight scenarios
   - Medium illumination: Replicating standard indoor lighting
   - Low illumination: Representing dim environment conditions

## 📁 Dataset Structure
The dataset follows the standard YOLO format organization for direct training compatibility:
```
dataset_root/
  ├── images/                # Image directory
  │   ├── 1.jpg
  │   ├── 2.jpg
  │   └── ...
  ├── labels/                # Annotation directory
  │   ├── 1.txt
  │   ├── 2.txt
  │   └── ...
  └── README.md             # Dataset documentation
```

## 💾 Data Acquisition and Usage
### Download Information
- Catbox Link: https://files.catbox.moe/q7fwme.zip
- File Size: Approximately 100 MB (compressed)
- Format: ZIP archive

### Extraction Instructions
#### Linux/macOS Users
```bash
# Navigate to download directory
cd /path/to/download

# Extract dataset
unzip dataset.zip -d /path/to/destination

# Set appropriate permissions
chmod -R 755 /path/to/destination/dataset
```

#### Windows Users
1. Using GUI:
   - Right-click the ZIP file
   - Select "Extract to current folder" or specify target directory
   
2. Using Command Line:
```cmd
# Navigate to download directory
cd C:\path\to\download

# Using 7-Zip (pre-installation required)
7z x dataset.zip -oC:\path\to\destination
```

## 👤 Data Collection Team
- Primary Collector: Yuwei Gui ([GitHub](https://github.com/vvamanda))

## 🎯 Application Scenarios
1. Robotic Visual Navigation
2. Autonomous Target Tracking
3. Real-time Object Detection
4. Robot-Object Interaction
5. Computer Vision Algorithm Testing

## 📝 Annotation Format
YOLO format annotation files (.txt) are organized as follows:
- Line format: `<class> <x_center> <y_center> <width> <height>`
- All values are normalized coordinates relative to image dimensions

## 📚 Citation Format
If you use this dataset in your research, please cite it as follows:
```
@dataset{RobotVisionDataset2025,
  author       = {Yuwei Gui},
  title        = {Path Tracking Robot Vision Dataset},
  year         = {2025},
  institution  = {Queen Mary University of London},
  event        = {Winter Hack 2025'}
}
```

## 🔄 Change Log
- 2025.02: Initial release

## 🤝 Contribution Guidelines
Community contributions to enhance dataset quality are welcome:
1. Issue reporting
2. Annotation optimization
3. New data contributions
4. Documentation improvements
