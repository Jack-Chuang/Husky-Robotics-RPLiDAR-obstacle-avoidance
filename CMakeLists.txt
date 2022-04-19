cmake_minimum_required(VERSION 3.12)

project(ObstacleAvoidance
  LANGUAGES CXX
  VERSION 0.0.0)

find_package(RPLidar REQUIRED)

add_executable(obstacle_avoidance
  main.cpp
  # Add any other .cpp files here. If you make a .h/.cpp pair, you need to add the .cpp
  )

target_link_libraries(obstacle_avoidance RPLidar::RPLidar)
