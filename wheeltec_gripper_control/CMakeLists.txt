cmake_minimum_required(VERSION 3.10.2)
project(wheeltec_gripper_control)
unset( CATKIN_INSTALL_INTO_PREFIX_ROOT )

find_package(ament_cmake REQUIRED)

install(DIRECTORY config
  DESTINATION share/${PROJECT_NAME}
)

set(CMAKE_CXX_STANDARD 17)

ament_export_dependencies(${THIS_PACKAGE_INCLUDE_DEPENDS})

ament_package()