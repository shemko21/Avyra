
Group Members and roles:

1. Dickson Mbogo - Program Developer
2. Elisha Jilo - Electrical Systems Developer
3. Shem Koech - Mechanical Designer
4. Masika - Supervisor


# Avyra
Overview
An autonomous ground-based robot designed to detect and fill potholes on roads using computer vision. It operates without human control by scanning surfaces, identifying damage, and performing targeted filling to restore road continuity.

Working

Surface Scanning
A forward-facing camera captures continuous images of the road ahead. These images are fed into a processing unit.

Pothole Detection
Using computer vision (OpenCV), the system analyzes the frames to detect depressions in the surface. Techniques include grayscale conversion, edge detection, contour analysis, and texture analysis to distinguish potholes from shadows or stains.

Classification
The identified area is validated against set thresholds for depth, size, and contrast to confirm it is a pothole. False positives are rejected.

Positioning
Once confirmed, the robot navigates precisely over the pothole using coordinate mapping and internal positioning logic. Navigation algorithms ensure accurate alignment.

Filling Operation
A concealed mechanism is activated to release and evenly spread filling material (e.g., asphalt mix or paste) into the pothole. The process is controlled to prevent overflow or underfill.

Surface Verification
A secondary image is captured post-fill. If the surface appears uniform and level, the robot resumes movement. If not, additional filling is triggered.

Loop Execution
The robot continues scanning and filling as it advances along the designated path.


Links:
Trello; 
