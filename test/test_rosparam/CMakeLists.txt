cmake_minimum_required(VERSION 3.0.2)

project(test_rosparam)
find_package(catkin REQUIRED COMPONENTS rostest)
catkin_package()

if(CATKIN_ENABLE_TESTING)
  add_rostest(test/rosparam.test)

  catkin_add_nosetests(test)
endif()
