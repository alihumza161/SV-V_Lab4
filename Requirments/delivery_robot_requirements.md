| Req. ID | Requirement                                                                                                                                                | Priority |
| ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| R1      | The robot shall remain in the **IDLE** state when powered on and shall wait for a delivery request.                                                        | High     |
| R2      | Upon receiving a valid delivery request, the robot shall transition from **IDLE** to **NAVIGATING**.                                                       | High     |
| R3      | While navigating, the robot shall detect obstacles in its surroundings and transition to **AVOIDING_OBSTACLE** when an obstacle is detected.               | High     |
| R4      | After successfully avoiding an obstacle, the robot shall return from **AVOIDING_OBSTACLE** to **NAVIGATING** toward the destination.                       | High     |
| R5      | When the robot reaches the destination, it shall transition from **NAVIGATING** to **DELIVERING**.                                                         | High     |
| R6      | The robot shall complete the delivery process and transition to **RETURNING** when the package is successfully delivered.                                  | High     |
| R7      | If the battery becomes critically low during navigation, the robot shall stop the current delivery journey and transition to **RETURNING**.                | High     |
| R8      | When the robot reaches the warehouse while returning, it shall transition from **RETURNING** to **IDLE**.                                                  | High     |
| R9      | The robot shall not transition directly from **IDLE** to **DELIVERING** without first receiving a delivery request and navigating to the destination.      | High     |
| R10     | The robot shall not transition directly from **AVOIDING_OBSTACLE** to **DELIVERING**; it shall resume **NAVIGATING** before entering the delivery process. | High     |
