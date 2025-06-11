# autodocking_saver

Start the container
```bash
docker compose run --rm raspberry
```

Compile
```bash
cd sensing-rigs-ros2/ros2_ws && \
echo "export PIP_BREAK_SYSTEM_PACKAGES=1" >> ~/.bashrc && \
source ~/.bashrc && \
rosdep update && \
rosdep install -i --from-path src --rosdistro jazzy -y -r && \
colcon build --symlink-install && \
source install/setup.bash
```
