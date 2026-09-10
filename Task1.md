+Task 1 — Autonomous Architecture+
           >.<

Objective

    The objective is to select the most suitable autonomous sensing and
    computing architecture for the search-and-rescue drone.

    The drone has a maximum allowed mass of 2.5 kg, so the selected
    architecture must provide sufficient perception and computation while
    keeping weight and power consumption low.

    The five architectures provided in the task were evaluated using:

    - Compute capability
    - Power consumption
    - Mission suitability
    - Weight
    - Cost
   ----------*------*----------

Architectures Given

 Option> - Sensor - Perception - Computing Platform 

1. Waveshare IMX219-83 Stereo Camera - NVIDIA Jetson Orin Nano
2. OAK-D Lite + AI - Raspberry Pi 5 8GB 
3. D500 LiDAR + Arducam IMX219 Wide Angle - Raspberry Pi 5 8GB 
4. Waveshare IMX219-83 Stereo Camera - Raspberry Pi 5 8GB 
5. Intel RealSense D435i - NVIDIA Jetson Orin Nano 

 ----------*------*----------

 Weightage system For The Task

 Object(Person) detection - 35%(Raw input)
 Computation - 25%(Processing and Identification)
 Weight - 15%(Crucial for range)
 Power - 15%(For treachorous conditions)
 Cost - 10%(Money cus we broke!)

 -As we have 5 systems I will give 5 points 4 points etc to 1 point to determine the best.

 -- Object Detection

1. OAK-D Lite + Raspberry Pi 5 - 5 POINTS
2. Intel RealSense D435i + Jetson Orin Nano - 4 POINTS
3. Waveshare IMX219-83 Stereo Camera + Jetson Orin Nano - 3 POINTS
4. Waveshare IMX219-83 Stereo Camera + Raspberry Pi 5 - 2 POINTS
5. D500 LiDAR + Arducam IMX219 + Raspberry Pi 5 - 1 POINT

-- Compute / AI Capability

1. Intel RealSense D435i + Jetson Orin Nano - 5 POINTS
2. Waveshare IMX219-83 Stereo Camera + Jetson Orin Nano - 4 POINTS
3. OAK-D Lite + Raspberry Pi 5 - 3 POINTS
4. Waveshare IMX219-83 Stereo Camera + Raspberry Pi 5 - 2 POINTS
5. D500 LiDAR + Arducam IMX219 + Raspberry Pi 5 - 1 POINT

-- Power

1. D500 LiDAR + Arducam IMX219 + Raspberry Pi 5 - 5 POINTS
2. OAK-D Lite + Raspberry Pi 5 - 4 POINTS
3. Waveshare IMX219-83 Stereo Camera + Raspberry Pi 5 - 3 POINTS
4. Intel RealSense D435i + Jetson Orin Nano - 2 POINTS
5. Waveshare IMX219-83 Stereo Camera + Jetson Orin Nano - 1 POINT

--Weight

1. OAK-D Lite + Raspberry Pi 5 - 5 POINTS
2. Waveshare IMX219-83 Stereo Camera + Raspberry Pi 5 - 4 POINTS
3. D500 LiDAR + Arducam IMX219 + Raspberry Pi 5 - 3 POINTS
4. Intel RealSense D435i + Jetson Orin Nano - 2 POINTS
5. Waveshare IMX219-83 Stereo Camera + Jetson Orin Nano - 1 POINT

--Cost

1. D500 LiDAR + Arducam IMX219 + Raspberry Pi 5 - 5 POINTS
2. Waveshare IMX219-83 Stereo Camera + Raspberry Pi 5 - 4 POINTS
3. OAK-D Lite + Raspberry Pi 5 - 3 POINTS
4. Waveshare IMX219-83 Stereo Camera + Jetson Orin Nano - 2 POINTS
5. Intel RealSense D435i + Jetson Orin Nano - 1 POINT

Weighted Score = (Points / 5) × Weight

--> 1. OAK-D Lite + Raspberry Pi 5 8GB

(5/5 × 35) + (3/5 × 25) + (4/5 × 15) + (5/5 × 15) + (3/5 × 10)

= 35 + 15 + 12 + 15 + 6

= 83 POINTS

--> 2. Intel RealSense D435i + Jetson Orin Nano

(4/5 × 35) + (5/5 × 25) + (2/5 × 15) + (2/5 × 15) + (1/5 × 10)

= 28 + 25 + 6 + 6 + 2

= 67 POINTS

--> 3. Waveshare IMX219-83 Stereo Camera + Raspberry Pi 5

(2/5 × 35) + (2/5 × 25) + (3/5 × 15) + (4/5 × 15) + (4/5 × 10)

= 14 + 10 + 9 + 12 + 8

= 53 POINTS

--> 4. Waveshare IMX219-83 Stereo Camera + Jetson Orin Nano

(3/5 × 35) + (4/5 × 25) + (1/5 × 15) + (1/5 × 15) + (2/5 × 10)

= 21 + 20 + 3 + 3 + 4

= 51 POINTS

--> 5. D500 LiDAR + Arducam IMX219 + Raspberry Pi 5

(1/5 × 35) + (1/5 × 25) + (5/5 × 15) + (3/5 × 15) + (5/5 × 10)

= 7 + 5 + 15 + 9 + 10

= 46 POINTS

Final Ranking (O~O *drumroll please*)

1. OAK-D Lite + Raspberry Pi 5 8GB — 83 POINTS
2. Intel RealSense D435i + Jetson Orin Nano — 67 POINTS
3. Waveshare IMX219-83 Stereo Camera + Raspberry Pi 5 — 53 POINTS
4. Waveshare IMX219-83 Stereo Camera + Jetson Orin Nano — 51 POINTS
5. D500 LiDAR + Arducam IMX219 + Raspberry Pi 5 — 46 POINTS

 ----------*------*----------

 --> BONUS:

 How would you orient the cameras to get the best way?

  I would orient the camera angled downwards which will help to sense depth and our goal of looking for people and they will be below us but not completely down as that would compromise obstacle avoidance.

  Alternative
  Livox MID-360 + Jetson Orin Nano 8GB

  A better LIDAR and Good AI will help us with better obstacle avoidance and person identification and Lidar is the tech used for this in cars and drones but the D500 is not up to par for the job of identification.

