# 🔬 Research Experience {#research-experience}

### NVIDIA Open-H & Intelligent Medical Mechatronics Lab
*Research Assistant · Sep 2025 – Present*

- Developed a multi-motor endoscope teleoperation system: built a 4-axis DJI M2006 motor control system with a RoboMaster A board and a Python host program, achieved high-frequency closed-loop motor control over CAN bus, and integrated an Xbox controller for vector-based endoscope actuation and PWM lighting control.
- Designed a multimodal data acquisition pipeline (serial communication, data logging, CSV storage), resolving timestamp alignment and synchronization between variable-frame-rate video and fixed-rate sensor streams.
- Built an endoscope data-collection tool with a visual UI recording motor position, velocity and joystick control vectors; cleaned and standardized the data into imitation-learning datasets compatible with the LeRobot framework.
- Trained end-to-end imitation-learning policies with the OpenPi framework (π0.5 series models), configuring multi-source datasets and joint training, and improving convergence and generalization through analysis of loss curves and training logs.
- Deployed and validated an AI endoscope model on embedded hardware with real-time inference from visual and state inputs, forming a closed loop from image input to motor action output.

### Hong Kong RGC Joint-Funded Project: Vision-Language-Navigation (VLN) Robotic System for Constrained Curved Environments
*Sep 2025 – Present*

- Studied autonomous navigation with multimodal large models in constrained, curved environments, targeting the complex control requirements of flexible robots.
- Built an end-to-end VLN large-model control framework; developed a dual-motor teleoperation platform and designed a multimodal data acquisition system, addressing multi-source data alignment.
- Led model development and deployment on Linux, integrating natural-language instructions, visual perception and low-level motor control to map multimodal inputs directly to motor commands.
- Outcome: precise endoscope navigation and trajectory tracking inside constrained curved channels, moving beyond the limitations of traditional geometric modeling, with potential applications in medical and other complex settings; related work is under major revision at *IEEE Transactions on Robot Learning*.

### Beijing Municipal-Level Project: Automatic Maize Seed Damage Detection Device Based on Soft X-ray Imaging and Image Recognition
*Feb 2022 – Apr 2024*

- Built a soft X-ray imaging system combined with deep learning for automated, non-contact detection of internal damage in maize seeds, deployed end-to-end from visual recognition to sorting actuation.
- Responsible for system setup and model training: built and preprocessed a standardized annotated seed-damage dataset; optimized the YOLOv8 architecture and loss function to improve detection of fine cracks.
- Conducted ablation studies and metric evaluation; exported the model and integrated it with the sorting device to close the loop from recognition to actuation, supporting project acceptance and deployment.
