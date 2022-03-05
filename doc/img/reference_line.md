## Coordinate

#### uv

#### st
(s,t) relative to st itself.

#### coordinate transformation
The coordinate transformation of st to xy is achieved by translation and rotation.
* translation: x, y
* z is given by the road elevation
* rotation: geometry, superelevation

## Reference line
There are a total of 5 types of reference lines "line, spiral, arc, poly3, paramPoly3"

#### line
Get the s-t coordinates first, then add the transformation

#### spiral & arc
First you need to get s-t according to the length, which requires some mathematical formulas

#### poly3 & paramPoly3
We do not currently support these two formats, because the coordinates need to be calculated according to the length


## Todo
1. support poly3 & paramPoly3
2. debug mode support `if __debug__:`

#### next
1. add predecessor_id, successor_id, left_neighbor_forward_lane_id, right_neighbor_forward_lane_id
2. lane LaneTurn
3. junctions
4. signal


## reference
https://releases.asam.net/OpenDRIVE/1.6.0/ASAM_OpenDRIVE_BS_V1-6-0.html#_coordinate_systems
https://docs.python.org/3/library/xml.etree.elementtree.html
