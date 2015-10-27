# ROS-Industrial Developer Meeting Notes

----------
**Date:** 10/13/2015

**Attendees:**

 - Craig Schlenoff
 - Risto Kojcev
 - Paul Hvass
 - Christina Gomez
 - Clay Flannig
 - Lars Tingelstad
 - Chris Lewis
 - Fred Proctor
 - Gijs vd. Hoorn
 - Levi Armstrong
 - Thomas Timm Andersen
 - Tom Panzarella
 - Mirko Bordignon
 - Frantisek Durovsky
 - Isaac Saito
 - Victor Lamoine
 - Pablo Quilez

**Agenda:** [Slides](meeting_agenda.pptx)

**Notes:**

 - Repository Status
     - [industrial_core](https://github.com/ros-industrial/industrial_core): Core industrial library for robot drivers and comms.
         - Release status:
             - indigo - released
             - jade - set to release (same as indigo)
         - Upcoming development:
             - jade release
     - [crcl](https://github.com/ros-industrial/crcl): Canonical Robot Command Language - provides generic command and status definitions that implement the functionality of typical industrial robots
         - Release status: N/A 
     - [fanuc](https://github.com/ros-industrial/fanuc): Support for fanuc robots
         - Release status:
             - indigo - released
             - jade - waiting on industrial_core
         - Upcoming development:
             - Multi-group control
             - Detailed meshes
     - [industrial_calibration](https://github.com/ros-industrial/industrial_calibration): Contains libraries/algorithms for calibration industrial systems
         - Release status:
             - indigo - source (unstable)
             - hydro - source (stable)
         - Upcoming development
             - New automated method for instrisic camera calibration (provides stable camera parameters)
     - [robot\_movement\_interface](https://github.com/ros-industrial/robot_movement_interface): Drivers implementing the Robot Movement Interface, which allows access to robot specific capabilities in a standardized common format while maintaining compatibility with the ROS-Industrial Joint interface.
         - Release status:
             - indigo - source release planned
         - Upcoming develpment
             - Porting existing code from internal IPA repo
     -  [ros_canopen](https://github.com/ros-industrial/ros_canopen): Canopen implementation for ROS.
         -  Release status
             -  indigo - released (stable)
         -  Upcoming development
             -  Expanding support for new devices (mostly drives)
             -  Support for ROS Control
     -  [industrial_moveit](https://github.com/ros-industrial/industrial_moveit): Contains packages that are meant for use with the MoveIt packages.
         -  Release status
             -  indigo - source (unstable)
         -  Upcoming development
             -  STOMP Planner improvements: see [video](https://www.youtube.com/watch?v=AvFoskssvVQ)
     -  [universal_robot](https://github.com/ros-industrial/universal_robot): Universal robots drivers
         -  Release status
             -  indigo - stable (except for new controllers)
         -  Upcoming development
             -  Integrated ros control
             -  bug fixes
     -  [abb](https://github.com/ros-industrial/abb): ABB robot drivers
         -  Release status
             -  indigo - released (stable)
     -  [motoman](https://github.com/ros-industrial/motoman):  Motoman robot dirvers
         -  Release status
             -  indigo - source (unstable)
         -  Upcoming development
             -  Update documenation
     -  [kuka(experimental)](https://github.com/ros-industrial/kuka_experimental): Kuka robot drivers
         -  Release status 
             -  indigo - experimental
         -  Upcoming development
             -  integrating Lwr4+ (Centre E. Piaggio)
             -  integrating IPA's work
     -  [robotiq](https://github.com/ros-industrial/robotiq): Robotiq gripper and force/torque sensor drivers
         -  Release status
             -  indigo - source (stable)
         -  Upcoming development
             -  Create a binary release [#42](https://github.com/ros-industrial/robotiq/issues/42)
     -  [siements(experimental)](https://github.com/ros-industrial/siemens_experimental): Support for siemens ProfiNET netowrks
         -  Release status
             -  hydro - source (unstable)
     -  [staubli](https://github.com/ros-industrial/staubli): Staubli robot drivers
         -  Release status
             -  No releases
         -  Upcoming development
             -  Initial driver release
     -  [bezier](https://github.com/ros-industrial-consortium/bezier): 5D tool path planner
         -  Release status
             -  Source is stable (not tied to ROS release (yet))
         -  Upcoming development
             -  Integration with Descartes
 -  New development
     -  [CAD to ROS](http://rosindustrial.org/events/2015/10/31/cad-to-ros-workbench-milestone-1-launch-anticipated) - New ROS-Industrial Consortium project started to create ROS workbench.  Has a hybrid open/closed source model
         -  See [roadmap](https://github.com/ros-industrial-consortium/roadmapping/blob/master/RoadmappingDocument.md#63-workspace-modeling) for more info.
     -  ROS [GPIO](https://en.wikipedia.org/wiki/General-purpose_input/output) support - support for general purpose (PC) IO.
     -  ROS for PLC - Utilize C-ROS library to create ROS applications on PLC platforms (a replacement to ladder logic).
         -  ROS OPC UA - See [article](https://github.com/ros-industrial-consortium/articles/blob/master/ros_with_opc-ua.md) by Mirko.
     -  ROS 2.0 (ran out of time)
 -  Action Items
     -  Send out meeting minutes
     -  Schedule next meeting
     -  Consider creating mailing list for developer discussion

