# Prototype Toolbox for Angle Cable Nutrunner Tensor STR

## Overview
The Prototype Toolbox for Angle Cable Nutrunner Tensor STR is a hardware integration project designed to enhance manual screw-tightening operations in industrial settings. This project involved developing a custom HAT (Hardware Attached on Top) attachment for the Raspberry Pi Compute Module 4 (CM4) that interfaces with a nutrunner and captures live video feeds for real-time monitoring.

The live video feed is utilized as input for the company's machine learning (ML) software, enabling accurate error detection during manual operations on the assembly line.

## Features
- **Custom HAT Design**: Designed a CAD-modelled HAT attachment that seamlessly integrates the Raspberry Pi CM4 with the nutrunner and CAM interface.
- **Real-Time Video Streaming**: Programmed the microcontroller to facilitate live video feed capture for monitoring and analysis.
- **Compact Form Factor**: Developed a small footprint enclosure to house the Raspberry Pi CM4, camera module, and custom circuitry for industrial applications.
- **Integration with ML Pipeline**: Provided video feed as input for the company’s existing ML pipeline, contributing to improved error detection in manual operations.

## Workflow
1. **HAT Attachment Design**:
    - Created a custom HAT attachment using CAD software to fit the Raspberry Pi CM4 and connect with the nutrunner.
    - Ensured proper alignment and connectivity for seamless operation.

2. **Microcontroller Programming**:
    - Programmed the Raspberry Pi CM4 to handle video capture from the camera module.
    - Developed the necessary scripts for real-time video streaming to monitor screw-tightening processes.

3. **Enclosure Development**:
    - Designed a compact enclosure that accommodates the Raspberry Pi CM4 and CAM interface, ensuring durability and easy mounting on the assembly line.

4. **Integration with ML Software**:
    - Provided the live video feed as input to the company's ML software, enhancing the system’s capability to detect errors during manual operations.

## Hardware & Tools
- **Raspberry Pi CM4**: The main video capture and control processing unit.
- **Raspberry Pi Camera Module (RPI CAM)**: Captures live video feeds for monitoring.
- **Custom HAT**: Enables seamless interfacing with the nutrunner and integrates necessary components.
- **CAD Software**: Used for designing the HAT attachment and enclosure.
- **Programming Language**: Python scripts for camera control and video streaming.

## Installation and Setup
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/TheMechanicHulk/Nutrunner-Prototype-Toolbox.git
    cd Nutrunner-Prototype-Toolbox
    ```

2. **Hardware Setup**:
    - Assemble the components according to the design specifications.
    - Mount the Raspberry Pi CM4 and CAM module onto the custom HAT.

3. **Software Configuration**:
    - Install required libraries on the Raspberry Pi:
    ```bash
    sudo apt update
    sudo apt install python3-opencv
    ```

4. **Run the Video Capture**:
    - Start the video streaming process:
    ```bash
    python3 video_capture.py
    ```

## Design Files
- **CAD Models**: The CAD files for the HAT attachment and enclosure can be found in the `cad/` folder.
- **Schematic Diagrams**: Include circuit schematics showing the connections between the Raspberry Pi CM4, CAM, and nutrunner.

## Results
- The developed prototype successfully captured live video feeds, providing real-time monitoring capabilities for the assembly line.
- Integration with the company's ML pipeline enabled enhanced error detection, improving operational efficiency.

## Future Improvements
- **Enhanced Video Processing**: Future work could include implementing real-time video processing algorithms for immediate error detection.
- **Wireless Communication**: Explore adding wireless capabilities for remote monitoring and data transmission.
- **Advanced ML Integration**: Collaborate with the ML team to refine input formats and enhance the predictive capabilities of the existing models.

## File Structure
```bash
├── cad/               # Contains CAD models and design files for the HAT and enclosure
├── scripts/           # Python scripts for video capture and processing
├── hardware/          # Instructions for hardware setup and assembly
└── README.md          # Project documentation
