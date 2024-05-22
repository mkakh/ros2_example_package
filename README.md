# ROS2のパッケージのサンプル

## 概要
ROS2のパッケージの作り方を学ぶために、ChatGPTに生成させたサンプルパッケージです。

## 作成時に行ったこと
```
# ワークスペースの作成
$ mkdir -p ~/ros2_work_space/src
$ cd ~/ros2_work_space
$ colcon build
$ source install/setup.bash

# パッケージの作成
$ cd ~/ros2_work_space/src
$ ros2 pkg create --build-type ament_cmake example_package --dependencies rclcpp std_msgs

# Publisherノードの作成
$ vim ~/ros2_work_space/src/example_package/src/publisher.cpp

# Subscriberノードの作成
$ vim ~/ros2_work_space/src/example_package/src/subscriber.cpp

# launchの作成
mkdir ~/ros2_work_space/src/example_package/launch
vim ~/ros2_work_space/src/example_package/launch/launch.xml

# CMakeLists.txtの編集
$ vim ~/ros2_work_space/src/example_package/CMakeLists.txt

# ビルド
$ cd ~/ros2_work_space
$ colcon build
$ source install/setup.bash

# launchファイルの実行
$ ros2 launch example_package launch.xml
```




