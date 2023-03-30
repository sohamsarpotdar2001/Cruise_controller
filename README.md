# Cruise-control-design-using-PID
This project was about developing a simple cruise control system with PID controller for acheiving a fixed SetPoint velocity.

## The Model - 

<img src="https://user-images.githubusercontent.com/92629417/228837521-b6a6ce81-c44d-47e9-b538-1621849f3edd.png" width="800" height="600"/>

If the inertia of the wheels is neglected, and it is assumed that air drag (which is proportional to the car’s speed at low speeds) is opposing the motion of the car, then the problem is reduced to a simple first order system.

Thus the motion of the car can be written as, **mv' + bv = u** where u is the input force provided by the engine to move the car at a certain velocity. Though it is intuitive to think of an input as something related to the gas pedal, but unfortunately to represent such a system accurately the dynamics of it become very complicated. Here we assumed that our engine can give us a certain amount of force, neglecting how that force translates to real life situations.


## Results

- Parameters - 
  - Mass m = 50
  - Drag Coefficient b = 30
  - SetPoint velocity = 150m/s
  
### Velocity v/s Time plot :
<img src="https://user-images.githubusercontent.com/92629417/228913154-25ae003a-53b0-44b7-92c5-731699f6d05a.png" width="800" height="600"/>

### Error v/s Time plot :
<img src="https://user-images.githubusercontent.com/92629417/228913350-e98b43a2-bc11-46df-b83d-7f81b92f57ff.png" width="800" height="600"/>

### Velocity & Error v/s Time:
<img src="https://user-images.githubusercontent.com/92629417/228821319-076d582c-a256-4c97-a976-de27ada97502.png" width="800" height="600"/>

### Conclusion
- Rise time of the system(time taken to reach 90% of the target velocity) = 4.6 seconds
- Maximum overshoot is less than 5%
