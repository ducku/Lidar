Using lidar data, return robot's position relative to the field

Guess and Check Boxes:
- Get previous position
- Use current Lidar data(theta, r, q)
- Draw box to limit area around previous position
    - An area the robot could’ve possibly have moved
- Cut area into 9 boxes
    - Loop through center of each box and check current lidar data (converted into x,y cord using hypothetical position) with previous lidar data(converted into x,y cords using previous position).
    - If most positions don’t have too many errors -> set that as current location or do it again but cut that area into 9 boxes again

Cons:
- Errors could accumulate
- Everything is relative
- Preferably have some methods of recentering or check position with the provided field map
