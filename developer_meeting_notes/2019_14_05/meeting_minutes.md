The primary discussion was on migration of ROS-Industrial Repositories to ROS2. There were a few approaches provided below and discussion will continue on discourse.

- The first was to keep everything in the same repository and leverage branches to separate ROS1 packages from ROS2
  - PROS
    - Only one repository
    - Easy to cherry pick features to other branches share the same history.
  - CONS
    - Maintainability is a concern. All issues and PR are inter mixed.
    - From the outside it may be confusing what branch/version they need
    - ROS Install will need to pull from multiple branches with namespaces
- The second was to keep the each in a separate repositories. Have a Library repository, ros1 wrapper repository, ros2 wrapper repository
  - PROS
    - Smaller code base easier to maintain.
    - PR's and issues are separated
    - Cherry pick features between ROS1 and ROS2 repository assuming share the same history
    - Each repository is specific to what it provides a developer (No confusion)
  - CONS
    - Multiple Repositories to maintain
