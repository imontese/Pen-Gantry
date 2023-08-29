# Project Title: HMI Controlled Motion Sequencer  
   
This project is an HMI controlled motion sequencer developed using Structured Text (ST) programming language. The sequencer controls the movement of a machine to different positions based on the selected points.  

## Motivation  
   
The motivation behind developing this HMI controlled motion sequencer is to provide an efficient and user-friendly way to control and automate the movement of machines in various applications. By enabling users to control motion through an HMI interface, it becomes easier to manage and monitor the machine's movements, reducing manual intervention and increasing productivity. This code can be particularly useful in industries where precise motion control is required, such as manufacturing, automation, and robotics.  
   
## Use Case: Automated Quality Inspection System  
   
One potential use case for this HMI controlled motion sequencer is in an automated quality inspection system used in a manufacturing plant. In this scenario, the system will be responsible for inspecting the quality of manufactured parts by moving a camera or sensor to different positions around the part to capture images or take measurements.  
   
To implement this system using the provided code, the following steps can be taken:  
   
1. Integrate the provided Structured Text code into a PLC or motion control system that supports Structured Text programming language.  
2. Configure the input and output variables according to the specific hardware and HMI setup, such as the motion control commands and part boundaries.  
3. Develop an HMI interface that allows users to input the desired inspection points and control the system using Home, Abort, and Start commands.  
4. Connect the camera or sensor to the motion control system, ensuring that the system can move the camera or sensor to the desired positions based on the selected inspection points.  
5. Implement additional logic in the PLC or control system to analyze the captured images or measurements and determine whether the inspected parts meet the quality criteria.  
   
By implementing this HMI controlled motion sequencer in an automated quality inspection system, it becomes easier for operators to manage and monitor the inspection process. This, in turn, helps to improve the overall efficiency of the production line and ensures that only high-quality products are shipped to customers.
   
## Features  
   
- Home position control  
- Abort command  
- Start command  
- Position search based on selected points  
- Motion control through different positions (Xmin, Ymin, Xmax, Ymax)  
- Commands to motion control to check if the desired position is reached  
   
## Code Structure  
   
The code is organized into different sections for better readability and maintenance:  
   
1. **Common**: This section initializes variables and timers, such as the step timer.  
2. **Control Sequencer**: This section defines the next step based on the input commands (Home, Abort, and Start) and the active step.  
3. **Sequencer / State Machine**: This section contains the logic for different steps in the sequencer, including:  
   - Home position  
   - Abort command handling  
   - Position search  
   - Movement through different positions (Xmin, Ymin, Xmax, Ymax)  
4. **Commands to Motion Control**: This section checks if the desired position is reached and manages the step timer.  
   
## Usage  
   
To use this code, integrate it into your PLC or motion control system that supports Structured Text programming language. Configure the input and output variables according to your specific hardware and HMI setup.  
   
Make sure to adjust the constants and parameters such as the number of parts, part boundaries, and motion control commands according to your application requirements.