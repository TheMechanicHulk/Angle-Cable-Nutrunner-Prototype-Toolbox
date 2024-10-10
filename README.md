# Prototype Toolbox for Angle Cable Nutrunner Tensor STR

## Overview
The Prototype Toolbox for Angle Cable Nutrunner Tensor STR is an innovative solution designed to enhance the quality control process in manual screw-tightening operations. This project involves developing a HAT (Hardware Attached on Top) attachment for the Raspberry Pi Compute Module 4 (CM4) and integrating a camera interface for live video feed capture. The captured video stream serves as an input for machine learning (ML) algorithms aimed at detecting errors during manual assembly.

## Features
- **CAD-Designed HAT Attachment**: Custom-designed HAT attachment to house the Raspberry Pi CM4 and Raspberry Pi Camera Module (RPI CAM).
- **Real-Time Video Streaming**: Programmed the microcontroller for seamless integration with the nut runner, enabling live video feed capture.
- **Machine Learning Integration**: Video feed is utilized by ML software for accurate error detection in manual screw-tightening operations.
- **Compact Design**: Developed a small footprint case to fit the given hardware for use in industrial assembly lines.

## Workflow
1. **CAD Design**:
    - Designed a compact HAT attachment using CAD software to accommodate the Raspberry Pi CM4 and RPI CAM.
    - Ensured the design met the dimensions and requirements of the industrial tool used on the assembly line.

2. **Hardware Integration**:
    - Integrated the Raspberry Pi CM4 and RPI CAM with the nut runner, allowing for real-time video capture.
    - Developed a custom HAT to facilitate communication between the camera, microcontroller, and the nut runner.

3. **Microcontroller Programming**:
    - Programmed the Raspberry Pi CM4 to handle video streaming and data processing tasks.
    - Ensured seamless interfacing between the components, allowing for reliable performance during operations.

4. **Machine Learning Pipeline**:
    - Utilized the captured video feed as input for ML algorithms designed to detect errors in screw-tightening operations.
    - Implemented software to analyze the video stream in real-time, providing immediate feedback on the assembly process.

## Hardware & Tools
- **Raspberry Pi CM4**: The main processing unit for handling video streams and interfacing with the nut runner.
- **Raspberry Pi Camera Module (RPI CAM)**: Used for capturing live video feeds.
- **Custom HAT**: Designed to integrate the camera and microcontroller efficiently.
- **CAD Software**: For designing the HAT and casing.
- **Python**: For programming the Raspberry Pi and implementing the video processing pipeline.

## Installation and Setup
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/TheMechanicHulk/Angle-Cable-Nutrunner-Prototype-Toolbox.git
    cd Angle-Cable-Nutrunner-Prototype-Toolbox
    ```

2. **Hardware Assembly**:
    - Assemble the components according to the CAD design specifications.
    - Ensure proper connections between the Raspberry Pi CM4, RPI CAM, and the nut runner.

3. **Software Installation**:
    - Install necessary libraries on the Raspberry Pi:
    ```bash
    sudo apt-get update
    sudo apt-get install python3-opencv
    pip install numpy
    ```

4. **Run the System**:
    - Start the video streaming process:
    ```bash
    python video_stream.py
    ```
    - The system will capture video feed and process it for ML error detection.

## Model Performance
- **Error Detection Accuracy**: The ML algorithms were trained using labeled video data, achieving a detection accuracy of over 90% in identifying errors during screw-tightening operations.
- **Real-Time Analysis**: The system provides real-time feedback, enhancing the quality control process in assembly lines.

## Results
- The prototype successfully integrates the Raspberry Pi CM4 and RPI CAM to capture live video feeds.
- The ML software effectively analyzes the video stream for error detection, improving operational efficiency and reducing defects in manual assembly.

## Future Improvements
- **Enhanced ML Algorithms**: Explore advanced ML techniques to improve error detection accuracy and speed.
- **Mobile App Integration**: Develop a mobile interface for remote monitoring and control of the assembly process.
- **User Interface Development**: Create a graphical user interface (GUI) for easier interaction and visualization of the system's performance.

## File Structure
```bash
├── data/              # Contains sample video data for training and testing ML models
├── models/            # Saved machine learning models
├── scripts/           # Python scripts for video streaming and ML integration
├── hardware/          # Instructions for hardware setup and CAD designs
└── README.md          # Project documentation
