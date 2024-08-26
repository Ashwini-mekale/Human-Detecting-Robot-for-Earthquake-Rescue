# HUMAN-DETECTING-ROBOT-FOR-EARTHQUAKE-RESCUE
---
# INTRODUCTION 
- A  new approach  for detecting  humans in  destructed environments  using  a autonomous  robot  is  proposed.

- Human  body  detection  system  proposed  a monitoring system  using sensors  and  camera  to capture, transmit  and  analyze conditions of human body.

- In order  to detect a human body , an autonomous robot must be equipped  with a specific  set of sensors  that provide  information about  the presence of a person  in the environment  around.

- Every year, various collapses of man-made structures such as bridges, buildings and also natural catastrophes like earthquake, landslides occur in various parts of the world. 

- This  system  has the  potential  to achieve high  performance in detecting   humans in  devastated  environments  relatively quickly  and cost-effectively.

- The Urban Search and Rescue (USAR) says, the probability of saving a victim is high only within the first 40hrs of rescue operation, and then the probability becomes zero. In such cases, humans are being trapped in the cavities created by collapsed building either in conscious or unconscious state.

- Disaster is a serious disruption of the functioning of a community or a society involving widespread human, material, economic or environmental losses and impacts, which exceeds the ability of the affected community or society to cope using its own resources.

# AIM AND OBJECTIVES
- The aim of this project is to build an efficient automated rescue robot to detect the human below the debris and to update the location via GPS. The objectives are as follows:

- Different Sensors are utilized in the project which in order to detect live humans. 

- To reduce the rescue operation time, and the number of rescue operators.

- To get an accurate location of a victim under surveillance.

- To get the data entity of the victim to know his/her condition, so that one can reach them as early as possible using web camera processing.

- To provide instance back support or force if necessary.

- To decrease the rate of deaths during natural calamity. 

## EXISTING SYSTEM
In this modern era of technology, still  conventional methods (human and trained dogs) are being used to find and rescue the victims who are buried under the rubble after natural or human-made destruction.

Such operation is very dangerous for the rescue workers and victims as well, especially in the case, if the wreckage is dislocated.

## PROPOSED SYSTEM

A PIR (Passive Infrared sensor) is utilized in the project which emits IR (infrared rays) in order to detect live humans. As an alive human (body) emits thermal radiation.

Temperature sensor is used to measure the temperature of the victim.

A camera to capture and display data when sensor trigger it.

In this proposed system, Robotic arm will be mounted which can be able to move objects.

# SYSTEM ARCHITECTURE
![image](https://github.com/user-attachments/assets/ac7985ab-dfc7-459f-bd1b-bda6676f799a)

# COMPONENTS DESCRIPTION
## RASPBERRY PI:
- Raspberry Pi acts as an Operating system with 5V.
  
- It consists of 40 pins, out of it we use 28 pins as general purpose pins.
  
- It has the capacity of storing 1 to 1.2GB RAM memory.
  
- The inbuilt processor is Broadcom processor ,which processing is up to 1.2 to 1.5GHz.
  
- It has 16 to 32 GB flash memory.

     ![image](https://github.com/user-attachments/assets/11e9a946-6fcc-4728-a68f-0764b2531b3c)

## PIR SENSOR:
- An infrared sensor is an electronic device, that emits in order to sense some aspects of the surroundings.
  
- An IR sensor can measure the heat of an object as well as detects the motion.

- These types of sensors measures only infrared radiation, rather than emitting it that is called as a passive IR sensor.

- Usually in the infrared spectrum, all the objects radiate some form of thermal radiations. These types of radiations are invisible to our eyes, that can be detected by an infrared sensor.

    ![image](https://github.com/user-attachments/assets/f3d34617-3909-40b9-8bc3-cc3d3c92537a)
                     
## WIRELESS TRANSMISSION: 

The robot position is tracked between intermittent global localization to have an all time position estimate available to the robot.
- Using GSM based wireless system for the efficient communication. 

- The GPS receiver receives the Longitudinal and latitudinal value when the system detects the movement of the human body it sends the location details to the stations using GSM modem.

## BUZZER: 
- A buzzer or beeper is an audio signaling device, which may be mechanical, electromechanical, or piezoelectric. 

- Typical uses of buzzers and beepers include alarm devices, timers, and confirmation of user input such as a mouse click or keystroke.

    ![image](https://github.com/user-attachments/assets/84fa4e6e-5e26-49a0-b100-fd95665a71fb)

## MOTOR DRIVER: 
- The motor driver is used to operate the front and the rear DC motors which in turn control the motion of the robot. 

- It is actually a current amplifier and converts the low current signal coming from a controller and amplifies it to provide the high current required for running the DC motors. 

  ![image](https://github.com/user-attachments/assets/5858ebfb-9a67-4a0e-b58f-eaee0b87792c)


## CAMERA: 
- The camera is the eye for robot, call as rob vision helps in monitoring security system and also can reach into the places where the human eye cannot reach. 
- Captures images of the victims in disaster area, and it is displayed  on the PC at the Transmitter section.

   ![image](https://github.com/user-attachments/assets/6f51ce98-56d8-4503-9459-4f2a655d6ee7)


## TEMPERATURE SENSOR:
- A temperature sensor is an electronic device that measures the temperature of its environment and converts the input data into electronic data to record, monitor, or signal temperature changes.

- The temperature sensor here we are using is LM35 sensor.

- The temperature detects the temperature and transfer it to client for further action to proceed.

   ![image](https://github.com/user-attachments/assets/0e47824b-748e-41e8-a968-7896346f1866)

## ROBOTIC ARM: 
- The arm is the main section of the robotic arm and consists of three parts: the shoulder, elbow and wrist End Effector. 

- The end effector acts as the hand of the robotic arm. Controllers are the main processors of the robotic arms and act as their brains.

- A typical robotic arm is made up of seven metal segments, joined by six joints.

- The computer controls the robot by rotating individual step motors connected to each joint The robot uses motion sensors to make sure it moves just the right amount.

   ![image](https://github.com/user-attachments/assets/07ad1f85-d9f5-41d0-819d-a434303f5f2c)


## POWER SUPPLY:
- It is an electrical device that supplies electric power to an electrical load. The primary function of a power supply is to convert electric current from a source to the correct voltage, current and frequency power to load the power. 5V power supply is used in our project

   ![image](https://github.com/user-attachments/assets/1ad425f4-daa4-4309-92ca-664da00ea02f)



# MODULE DESCRIPTION 
1. Image Acquisition : 
         First step deals with acquiring the image by any one the devices, such as Handy Cam, Mobile Camera, USB camera and CCTV Camera etc.

2. Frame Conversion : 
         Once the image is captured, those images are converted into frames and suitable type of processing can be done conveniently.

3. Pre-Processing :
      Pre-processing is applied on the frames of the images. Some of the common methods of preprocessing are smooth, dilate, erode and median etc.

4. Background Modeling : 
     Once the pre-processing is done, background modeling is used to create an ideal background (static or dynamic) according to the environmental changes. Background Modeling important step of the system to perform some image subtraction operations. It is the default characteristics of any background subtraction system. According to the literature there are several background modeling techniques which are categorized as recursive or non-recursive techniques. For this system recursive technique being used.

5. Background Subtraction :
      This is the main step in the background subtraction system. In this step any significant changes in the image region from background model are identified & then pixels constituting the regions undergoing change are marked for further processing. Usually connected component labeling algorithm is applied to obtain connected regions corresponding to the object.

6. Post-Processing : 
         Finally, post-processing is done to improve the results. There are many post processing techniques that can be used after background modeling and subtraction. These techniques have an objective to improve foreground mask.

 7. Foreground Extraction : 
         This is the final step in the process which extracts the moving object from the frame. The result of this step helps in the judgment of the efficiency of the background subtraction system.

      ![image](https://github.com/user-attachments/assets/9c85b930-9c30-4d75-bfa2-cee3547b31fa)


# APPLICATIONS OF THE PROJECT
Robots  can perform variety of functions  independently.  General purpose  robots  may perform a variety of functions simultaneously or  they may take on different  roles at different times of day. This specific Rescue robot that has been designed for a specific purpose can be used for the following applications: 
- In disaster zones, whether it natural or man-made disaster.

- In Rescue operations where human reach is not possible.

- This helps to reduce the time, hence it is less time consuming.

- A camera is used to capture and can detect the person.

- As the Robot can move, it covers lot of distance that reduces the use of man power.


# CONCLUSION
- In this project, a new system and methodology for detecting surviving humans in destructed environments using an emulated autonomous robot is proposed.
- The goal of this was to provide a low cost rescue robot for human detection in a disaster environment.
- The sensors used in the development of this project are easily available and cost effective. It has a wide future scope.
- By this system, it will be a great help indeed to rescuers in detection of the human beings at the disaster sites. This is also user friendly, economical, semi-autonomous, and efficient device for detection of humans.


# SNAPSHOTS
Overview of the robot                                                                              


   ![image](https://github.com/user-attachments/assets/9a6644ea-bbc7-43a0-a317-17582d218b60)           


Front view of the robot

   ![image](https://github.com/user-attachments/assets/e2c5b277-44f6-475b-b5c4-c6fe9a8362ae)


   

Back view of the robot

   ![image](https://github.com/user-attachments/assets/307c0f95-22e8-44c8-9735-d1af32444884)


Image captured by camera



  ![image](https://github.com/user-attachments/assets/da37705d-bc26-4b6b-86be-81461572fea3)              ![image](https://github.com/user-attachments/assets/2eed5e0c-1a48-46e8-9887-f4d03b96997f)    


# REFERENCES
- R. Ventura, P.U. Lima, “Search and rescue robots: the civil protection teams of the future,” Third International Conference on Emerging Security Technologies (EST), 2012, pp. 12-19.

- M. Micire, “Analysis of the robotic-assisted search and rescue response to the world trade center disaster,” Master’s Thesis, University of South Florida, 2002.

- R. Murphy, “Rescue robots at the World Trade Center,” Journal of the Japan Society of Mechanical Engineers, Special issue on Disaster Robotics, 2003,102(1019), pp. 794-802.

- S. Tadokoro, Rescue Robotics: DDT Project on Robots and Systems for Urban Search and Rescue, Springer Dordrecht Heidelberg London New York, 2009.

- A. Jaroff, E. Messina, B. A. Weiss, S. Tadokoro, Y. Nakagawa, “Test arenas and performance metrics for urban search and rescue robots,” In Proc. of the 2003 IEEE/RSJ International Conference on Intelligent Robots and Systems, pp. 3396-3403.

- C. Schlenoff, H. Scott, S. Balakirsky, “Performance evaluation of intelligent systems at the national institute of standards and technology,” ITEA Journal, vol. 32, pp. 59–67, 2011..







