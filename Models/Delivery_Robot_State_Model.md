State_ID| State_Name| Description| Entry Condition| Exit Condition
S-01| IDLE| Robot is waiting for a delivery request.| The robot is powered on and no delivery request is active.| Transition to NAVIGATING when a delivery request is received.
S-02| NAVIGATING| Robot is travelling toward the destination.| A delivery request has been received and the robot has started moving to the destination.| Transition to AVOIDING_OBSTACLE when an obstacle is detected, to DELIVERING when the destination is reached, or to RETURNING when the battery is critically low.
S-03| AVOIDING_OBSTACLE| Robot is handling an obstacle detected during navigation.| An obstacle is detected while the robot is navigating.| Transition to NAVIGATING after the obstacle has been successfully avoided.
S-04| DELIVERING| Robot is performing the package delivery.| The robot has reached the destination and the delivery process begins.| Transition to RETURNING after the package is successfully delivered.
S-05| RETURNING| Robot is travelling back to the warehouse.| The package has been delivered or the battery is critically low and the robot must return.| Transition to IDLE when the warehouse is reached.

Events:
- Delivery Request Received
- Obstacle Detected
- Obstacle Avoided
- Destination Reached
- Delivery Successful
- Critical Battery
- Warehouse Reached
