| Transition ID | From State        | Event / Condition         | To State          | Requirement |
| ------------- | ----------------- | ------------------------- | ----------------- | ----------- |
| T1            | IDLE              | Delivery Request Received | NAVIGATING        | R2          |
| T2            | NAVIGATING        | Obstacle Detected         | AVOIDING_OBSTACLE | R3          |
| T3            | AVOIDING_OBSTACLE | Obstacle Avoided          | NAVIGATING        | R4          |
| T4            | NAVIGATING        | Destination Reached       | DELIVERING        | R5          |
| T5            | DELIVERING        | Delivery Successful       | RETURNING         | R6          |
| T6            | NAVIGATING        | Critical Battery          | RETURNING         | R7          |
| T7            | RETURNING         | Warehouse Reached         | IDLE              | R8          |
