pose_path_publisher
==============

1. About

    The pose_path_publisher package contains a ROS node that provides current position and orientation of the robot and it's path in the map or odometry frame. This package can be used in multi-robot systems.

2. Nodes

    2.1 pose_path_publisher
    
    pose_path_publisher provides current position and orientation of the robot and it's entire path in the map.

    2.1.1 Published Topics
    
    /pose (geometry_msgs/PoseStamped)
    /path (nav_msgs/PoseStamped)
    
    as the Current robot pose and path. 

    2.1.2 Parameters
    
      ~publish_frequency (double, default: 10.0)
      
        Frequency (HZ) at which to publish the robot pose and path. 

      ~map_frame (std::string, default: map)
      
        The frame attached to the map or odometry frame. 

      ~base_frame (std::string, default: base_link)
      
        The frame attached to the mobile base.
        
3. Usage

    roslaunch pose_publisher pose_publisher.launch

4. Related Documentation

    Please refer to the following paper to retrieve more information on the node:

    @inproceedings{yz14simpar,
    author = {Zhi Yan and Luc Fabresse and Jannik Laval and Noury Bouraqadi},
    title = {Team Size Optimization for Multi-robot Exploration},
    booktitle = {In Proceedings of the 4th International Conference on Simulation, Modeling, and Programming for Autonomous Robots (SIMPAR 2014)},
    pages = {438--449},
    address = {Bergamo, Italy},
    month = {October},
    year = {2014}
    }

5. Support

    Zhi Yan, Luc Fabresse, Jannik Laval, and Noury Bouraqadi
    Ecole des Mines de Douai, 59508 Douai, France
    http://car.mines-douai.fr

