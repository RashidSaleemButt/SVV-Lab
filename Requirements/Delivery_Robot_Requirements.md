Req ID| Description| Priority
R-01| The robot shall remain in the IDLE state while waiting for a delivery request.| High
R-02| Upon receiving a delivery request, the robot shall begin navigating toward the specified destination.| High
R-03| While navigating, the robot shall continuously monitor its surroundings for obstacles.| High
R-04| When an obstacle is detected during navigation, the robot shall enter obstacle-avoidance mode.| High
R-05| After successfully avoiding an obstacle, the robot shall resume navigation toward the destination.| High
R-06| When the destination is reached, the robot shall start the delivery process.| High
R-07| The robot shall not enter the delivery process directly from IDLE or obstacle-avoidance mode.| High
R-08| After successfully delivering the package, the robot shall begin returning to the warehouse.| High
R-09| When the battery becomes critically low during navigation, the robot shall stop the current delivery journey and return to the warehouse.| High
R-10| When the robot reaches the warehouse, it shall become IDLE and wait for another delivery request.| High
