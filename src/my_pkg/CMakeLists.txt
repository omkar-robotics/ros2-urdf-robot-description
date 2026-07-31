cmake_minimum_required(VERSION 3.8)
project(my_pkg)

if(CMAKE_COMPILER_IS_GNUCXX OR CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  add_compile_options(-Wall -Wextra -Wpedantic)
endif()

# Find dependencies
find_package(ament_cmake REQUIRED)

# Uncomment and add more dependencies here if needed
# find_package(rclcpp REQUIRED)
# find_package(robot_state_publisher REQUIRED)

if(BUILD_TESTING)
  find_package(ament_lint_auto REQUIRED)

  # Skip copyright check
  set(ament_cmake_copyright_FOUND TRUE)

  # Skip cpplint
  set(ament_cmake_cpplint_FOUND TRUE)

  ament_lint_auto_find_test_dependencies()
endif()

# Install the URDF folder
install(
  DIRECTORY urdf
  DESTINATION share/${PROJECT_NAME}
)

# Install the launch folder
install(
  DIRECTORY launch
  DESTINATION share/${PROJECT_NAME}
)

ament_package()
