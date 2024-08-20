cmake_minimum_required(VERSION 3.10.2)
project(wheeltec_hardware_interface)
unset( CATKIN_INSTALL_INTO_PREFIX_ROOT )

find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)

install(DIRECTORY launch config
  DESTINATION share/${PROJECT_NAME}
)

set(CMAKE_CXX_STANDARD 17)

ament_export_dependencies(${THIS_PACKAGE_INCLUDE_DEPENDS})

ament_package()