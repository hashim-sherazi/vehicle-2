# Braitenberg_Vehicles_unreal
## Braitenberg’s Vehicles: Exploration on Unreal Engine
Braitenberg Vehicles are a fascinating concept in the field of autonomous robotics that originated from the work of Italian neuroscientist Valentino Braitenberg. These vehicles demonstrate emergent behavior through simple sensor-motor connections, offering valuable insights into the complex relationship between perception, cognition, and action.

The essence of Braitenberg Vehicles lies in the interplay between sensors and actuators. The vehicles are equipped with sensors that gather information about their environment, and this sensory input is processed to produce motor commands that drive the vehicles' behavior. The behavior of each vehicle emerges from the specific connections and interactions between its sensors and actuators.

There are various sensor connections that can be implemented in Braitenberg Vehicles, each resulting in distinct behaviors. A commonly explored approach including scrub tracing involves a sensor positioned at the front of the vehicle, which detects and reacts to obstacles by "scrubbing" or making contact with them through a Sphere Trace.

We will explore five unique vehicles, each exemplifying different sensor connections and exhibiting their own emergent behaviors. By studying and modifying these vehicles, we will gain a deeper understanding of how sensor-motor connections influence their actions and interactions with the environment.

Through this exploration, we will uncover the intricacies of Braitenberg Vehicles and witness firsthand how even the simplest of connections can give rise to complex and adaptive behaviors. So, let's begin our journey into the captivating world of Braitenberg Vehicles and discover the remarkable potential of autonomous systems driven by sensor-motor relationships.

## Vehicle 1: Simplest possible vehicle equipped with one sensor and one motor. The sensor is directly connected to the motor. The sensor’s output is higher as it gets closer to the source.
Sensor Setup:

![image](https://github.com/ceciljoseph97/Braitenberg_Vehicles_unreal/assets/29672160/12e92e49-8f2f-42c9-8da9-fbb72f77f2a8)

## Vehicle 2: Two sensors and two motors. Cross Connection is employed. The vehicle heads towards sources, Throttle is higher as it gets closer to the source.
Sensor Setup:

![image](https://github.com/ceciljoseph97/Braitenberg_Vehicles_unreal/assets/29672160/d4bf6f6d-b603-4a79-a5c0-ac302d9a73f1)

## Vehicle 3: The vehicle has two types of sensors: one for Excitation and the other for inhibition.
Sensor Setup:

![image](https://github.com/ceciljoseph97/Braitenberg_Vehicles_unreal/assets/29672160/89de06ca-6bbe-47a5-a30a-fde024bdc5df)

## Vehicle 4: The vehicle sensors have nonlinear characteristics.
Sensor Setup(Similar to vehicle 3):

![image](https://github.com/ceciljoseph97/Braitenberg_Vehicles_unreal/assets/29672160/344aa561-2230-4e38-a882-1040b620f7ef)

Non-linearity in the sensory input is enforced using functions like ReLU, sigmoid, and classic step functions, complemented with logarithmic transformations. Notably, vehicle 4 exhibits a more stable throttle input, showcasing differences in behavior compared to other vehicles.


## Vehicle 5: The Vehicle Learns to control its Throttle Output, employing a neural Component to learning throttle weight.
Sensor Setup(Similar to Vehicle one):

![image](https://github.com/ceciljoseph97/Braitenberg_Vehicles_unreal/assets/29672160/c5cc1db6-404e-4319-b712-e0e08b4c205b)

Get Throttle Input: We use Get Throttle Input from the NeuralComponent Through a Forward pass.
![image](https://github.com/ceciljoseph97/Braitenberg_Vehicles_unreal/assets/29672160/40f46656-ba2c-4553-b7be-76002a7a36b5)

# Easy Demonstration 
Step 1: In ThirdPersonMap, Hit play -> Visit the Levels through the level Portal for Implementation Through Scrub Tracing.

![image](https://github.com/ceciljoseph97/Braitenberg_Vehicles_unreal/assets/29672160/ce4fa8e3-d1bd-4c0c-8ad8-9f356dee4a62)

For Advanced view 

![image](https://github.com/ceciljoseph97/Braitenberg_Vehicles_unreal/assets/29672160/c3f7bb45-e62c-4f89-b231-cdf78217df5c)

In Level 1, the car behavior is controlled by Key Stroke 2, while the player is controlled by Key Stroke 1. Key Stroke 3 activates Manny1Excitatory, which is also applicable to Level 2. Key Stroke 4 triggers Manny2Inhibi.

In Levels 2, 3, 4, and 5, the car is controlled by Key Stroke 2, and the player is controlled by Key Stroke 1.





