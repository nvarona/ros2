# URDF Example


Este repositorio contiene un ejemplo de un archivo URDF y un script de inicio para ejecutarlo. (ROS 2)
Esto es parte de un tutorial sobre la creación de archivos URDF, disponible en los enlaces siguientes:

YouTube:

Blog Post:

## Como ejecutar

1. Construya el paquete con colcon.
2. Inicie el archivo de inicio `robot_state_publisher` con `ros2 launch urdf_example rsp.launch.py`.
3. Inicie `joint_state_publisher_gui` con `ros2 run joint_state_publisher_gui joint_state_publisher_gui`. Es posible que necesites instalarlo si aún no lo tienes.
4. Inicie RViz con `rviz2`

Para replicar la pantalla RViz, querrás:
- Establece tu marco fijo en "mundo"
- Agregue una visualización `RobotModel`, con el tema establecido en `/robot_description` y alfa establecido en 0,8
- Agregue una pantalla `TF` con nombres habilitados.

## How To Run

1. Build the package with colcon.
2. Launch the `robot_state_publisher` launch file with `ros2 launch urdf_example rsp.launch.py`.
3. Launch `joint_state_publisher_gui` with `ros2 run joint_state_publisher_gui joint_state_publisher_gui`. You may need to install it if you don't have it already.
4. Launch RViz with `rviz2`

To replicate the RViz display, you will want to
- Set your fixed frame to `world`
- Add a `RobotModel` display, with the topic set to `/robot_description`, and alpha set to 0.8
- Add a `TF` display with names enabled.
