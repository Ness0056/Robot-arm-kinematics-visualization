# Robot Arm Kinematics Visualization

A 3D robotic arm simulation developed using **POV-Ray** and the
**Denavit–Hartenberg (DH) convention**.

The project demonstrates how a multi-link robotic manipulator can be
constructed using chained rotations and translations. By changing the
joint angles over time, the model can also be animated to visualize the
motion of the robot arm.

## Overview

Each link of the robot is represented using Denavit–Hartenberg parameters.

The transformations are applied sequentially so that the position and
orientation of each link depend on the previous link. This creates the
kinematic chain of the robotic arm.

The project includes:

- 3D robotic arm modelling
- Denavit–Hartenberg parameters
- Chained coordinate transformations
- Multiple joint configurations
- Animated joint movement
- POV-Ray rendering

## Technologies

- POV-Ray
- 3D Geometry
- Robot Kinematics
- Denavit–Hartenberg Convention
- Homogeneous Transformations

## Robot Kinematics

The position of every robot link is obtained by applying a sequence of
rotations and translations.

Using the Denavit–Hartenberg convention, each joint can be described using
a small set of parameters defining the relationship between consecutive
coordinate systems.

The transformations are then chained together to obtain the complete
pose of the robotic arm.

## Animation

The joint angles are varied using POV-Ray's animation clock.

For example:

```pov
#declare Fi1 = 30*clock;
#declare Fi2 = 60*clock;
#declare Fi3 = 40*clock;
```

As `clock` changes during rendering, the angles of the joints change,
producing the movement of the robotic arm.

## Demo

▶️ [Watch the full robot arm animation](animation/animation.mp4)
