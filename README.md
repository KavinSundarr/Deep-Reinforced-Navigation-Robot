
# DRL_Navigation_Robot_ROS2_Foxy

**Abstract**  
This project demonstrates a mobile robot, equipped with a LIDAR sensor, trained to navigate to random goal points in a simulated environment while avoiding obstacles. The robot was trained using Deep Reinforcement Learning (DRL) with the Twin Delayed Deep Deterministic Policy Gradient (TD3) algorithm. The implementation leverages the ROS Gazebo 11 simulator for training and ROS2 Foxy for testing. PyTorch was used to develop the neural network models, and Tensorboard provided real-time monitoring during training. The robot achieved a navigation accuracy of 82%, highlighting the efficacy of the TD3 method in enhancing autonomous navigation capabilities.

**Key Highlights**  
- **Training**: Conducted in ROS Gazebo 11 using TD3 with PyTorch.
- **Testing**: Performed in ROS2 Foxy on Ubuntu 20.04.
- **Algorithm**: The TD3 architecture includes an actor-network for action selection and two critic networks to minimize Q-value overestimation.
- **Monitoring**: Training progress visualized in real-time with Tensorboard.

**How to Use**  
1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/DRL_Navigation_Robot_ROS2_Foxy.git
    cd DRL_Navigation_Robot_ROS2_Foxy
    ```

2. **Build the workspace**:
    ```bash
    source /opt/ros/foxy/setup.bash
    colcon build
    source install/setup.bash
    ```

3. **Train the robot**:
    ```bash
    ros2 launch td3 training_simulation.launch.py
    ```

4. **Monitor training with Tensorboard**:
    ```bash
    tensorboard --logdir ./src/td3/runs/train/tensorboard
    ```

5. **Test the robot**:
    ```bash
    ros2 launch td3 test_simulation.launch.py
    ```

**Visuals**  
![Training Example](https://github.com/toxuandung/DRL_Navigation_Robot_ROS2_Foxy/blob/main/Training_example.gif)

![Testing Example](https://github.com/toxuandung/DRL_Navigation_Robot_ROS2_Foxy/blob/main/Test_example_env1.gif)

**Conclusion**  
This project demonstrates the potential of DRL in robotic navigation, with the TD3 algorithm proving effective in enabling the robot to navigate autonomously in complex environments. With an 82% navigation accuracy, this work lays the groundwork for future advancements in autonomous navigation systems.
"""

# Saving the refined content into a new README.md file
output_file_path = '/mnt/data/README_refined.md'

with open(output_file_path, 'w') as file:
    file.write(refined_readme_content)

output_file_path
