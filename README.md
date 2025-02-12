# Mechanum Drive Tank
## ECE 4180 Final Project S23
### Oscar Baglivio, Ray Daw, Yunhao Hu, Steven Zhao

**Mechanum Drive Wheels** are designed similarly to tank wheels, allowing our vehicle to move forward and backward, as well as turn, but what makes them unique is the added ability to "strafe" or move side to side. This is thanks to the diagonal rollers, meaning that the wheels can exert force in the diagonal direction. With the proper combination of these forces, our vehicle can move **forward, backward, left, right**, as well as **rotate** about the **center** or **edge** of the vehicle.

<img width="230" alt="Screen Shot 2023-04-28 at 2 22 03 PM" src="https://user-images.githubusercontent.com/113135441/235224360-a8931893-abb8-4909-a532-3a1c8ad1d264.png">

## Drive Modes
Our drive modes will be toggled in a state machine as follows:
<img width="520" alt="Screen Shot 2023-04-28 at 2 31 21 PM" src="https://user-images.githubusercontent.com/113135441/235226007-f9ad2847-7def-4ca9-96de-c2296dda2b6e.png">
### Translational
**Translational Mode** allows the vehicle to move linearly foward, backward, right, and left.
### Diagonal
**Diagonal Mode** allows the vehicle to move linearly towards the upper right, upper left, lower right, and lower left.
### Tank
**Tank Mode** allows the vehicle to move linearly foward/backward and rotate about its center clockwise/counterclockwise (similar to a tank).
### Driving
**Driving Mode** allows the vehcile to move linearly foward/backward and turn about the rear axis left/right (similar to a standard car).

## Controls
The vehicle will be controlled via the adafruit bluefruit bluetooth module coonnected to the BluefruitConnect app with the following controls:

<img width="442" alt="Screen Shot 2023-04-28 at 2 52 15 PM" src="https://user-images.githubusercontent.com/113135441/235229974-18c711cd-7dcc-404d-bbc3-14bc213e8f87.png">

#### Directional Controls
| Button      | Translational | Diagonal | Tank | Driving |
| ----------- | ----------- | ----------- | -------- | -------- |
| Up          | Forward     |Forward/Left|Forward      |Forward       |
| Down        | Backward    |Backward/Right|Backward       |Backward       |
| Right       | Right Linear|Forward/Right|Clockwise Rotate |Right Turn      |
| Left        | Left Linear |Backward/Left|Counterclockwise Rotate|Left Turn       |
#### Number Pad Controls
| Number Pad      | Function
| ----------- | ----------- | 
| 1           | Mode Toggle   |   
| 2           | Auto Toggle   |  
| 3           | Decrease Speed |
| 4           | Inrease Speed   |    
