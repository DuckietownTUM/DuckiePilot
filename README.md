# DuckiePilot

DuckiePilot is an autonomous navigation project developed on the Duckietown platform.  
The system demonstrates key concepts of self-driving systems by integrating perception, decision-making, and control into a compact robotic platform.

---

## Overview

This project implements a modular pipeline for autonomous navigation:

- **Perception**: Interpreting visual input from the onboard camera  
- **Decision-Making**: Determining appropriate actions based on environment  
- **Control**: Executing motion commands through motor actuation  

The system is designed to operate in a structured Duckietown environment and handle common driving scenarios.

---

## Key Features

### Lane Following
- Real-time lane detection using camera input  
- Estimation of lateral offset and heading error  
- PID-based control for smooth and stable motion  
- Continuous correction to maintain lane alignment  

---

### Intersection Navigation
- Detection of intersections using visual cues (e.g., stop lines, markers)  
- Decision logic for maneuver selection (left, right, straight)  
- Controlled execution of turns  
- Seamless transition back to lane-following mode  

---

### Obstacle Detection and Safety Response
- Real-time object detection using a YOLOv5-based model  
- Identification of relevant obstacles (e.g., ducks, other Duckiebots)  
- Safety mechanism to halt the robot when an obstacle is detected in its path  

---

## System Architecture

The system follows a layered architecture:

1. **Perception Layer**  
   Processes camera input to extract lane and object information  

2. **Decision Layer**  
   Handles behavioral logic for navigation and safety  

3. **Control Layer**  
   Converts decisions into motor commands using feedback control  

---

## Technologies Used

- Python  
- Duckietown Software Stack  
- OpenCV (image processing)  
- YOLOv5 (object detection)  
- PID Controller (feedback control system)  

---

## Demonstration

The demonstration video showcases:
- Lane-following behavior under continuous correction  
- Navigation through an intersection scenario  
- Obstacle detection with stopping response   

---

## Challenges

- Reliable system integration across perception, control, and detection modules  
- Parameter tuning for stable motion and responsiveness  
- Handling environmental variability (e.g., lighting conditions, camera input noise) during testing   

---

## Future Work

- Extension to dynamic obstacle avoidance  
- Improved robustness under varying lighting and environmental conditions  
- Enhanced intersection handling strategies  
- Multi-agent coordination and advanced path planning  

---

## Authors

- Shivam Bhatt
- Hejunjie Cao
-Shibin Dong
 

---

## Acknowledgments

This project builds upon the Duckietown platform and leverages open-source tools and resources provided by the Duckietown community.

## Project Report

[Final Report (PDF)](docs/report/Report.pdf)

---

## Presentation Slides

[Final Presentation (PPT)](docs/presentation/Slides.pptx)

---

## Demo Video

[Watch Demo Video](https://youtu.be/UdbZ-b8Hbuk)

---

## References

- Duckietown Platform  
- Duckietown TUM
