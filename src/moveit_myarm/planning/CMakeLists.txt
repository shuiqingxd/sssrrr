add_executable(planning_scene src/planning_scene.cpp)
target_link_libraries(planning_scene ${catkin_LIBRARIES} ${Boost_LIBRARIES})
install(TARGETS planning_scene DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})

add_executable(planning_scene_ros_api src/planning_scene_ros_api.cpp)
target_link_libraries(planning_scene_ros_api ${catkin_LIBRARIES} ${Boost_LIBRARIES})
install(TARGETS planning_scene_ros_api DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})

#add_executable(motion_planning_api_tutorial src/motion_planning_api_tutorial.cpp)
#target_link_libraries(motion_planning_api_tutorial ${catkin_LIBRARIES} ${Boost_LIBRARIES})
#install(TARGETS motion_planning_api_tutorial DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})
#
#add_executable(planning_pipeline_tutorial src/planning_pipeline_tutorial.cpp)
#target_link_libraries(planning_pipeline_tutorial ${catkin_LIBRARIES} ${Boost_LIBRARIES})
#install(TARGETS planning_pipeline_tutorial DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})

add_executable(group_interface src/group_interface.cpp)
target_link_libraries(group_interface ${catkin_LIBRARIES} ${Boost_LIBRARIES})
install(TARGETS group_interface DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})

install(DIRECTORY launch DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
#install(PROGRAMS
#  scripts/move_group_python_interface_tutorial.py
#  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
#)
