# Writeup: 3D Object Detection

## Vary degrees of visibility of vehicle
Trying to identify vehicles in a point-cloud can be trivial. Some vehicles are clear enough to determine not only that a
vehicle is in that location, but also things like what type of vehicle it is.

Other vehicles can be found without too much trouble, but have some features obscured, which might be detrimental
to a neural network's ability to identify them.

Finally, some vehicles are difficult to find - due to obstructions, distance, or even awkward angle - even for a human.

### Easily Identifiable Vehicles
![](/img/clearlyVisible1.png)
![](/img/clearlyVisible2.png)
![](/img/clearWithTow.png)


### Moderate Visibility Vehicles
![](/img/truck.png)
![](/img/partiallyObscured1.png)
![](/img/partiallyObscured2.png)
![](/img/clearlyVisible1.png)
![](/img/clearlyVisible2.png)
![](/img/tooClose.png)

### Difficult Vehicles
![](/img/difficultToSee.png)
![](/img/visibleButDistant.png)

## Identifiable Features of Vehicles
By far the most clearly identifiable feature for lidar detection is the reflectors by the taillights of vehicles. 
Admittedly, this isn't exactly the most shocking revelation, as the lidar works by detecting light that reflects back to it.
License plates were also a very prominent feature, because they are also fairly reflective. Suprisingly, headlights were
not consistently clear. 


![Rear Reflectors and License Plates are clearly visible](/img/rearReflectors.png)
![Headlights are not clear](/img/noHeadlights.png)