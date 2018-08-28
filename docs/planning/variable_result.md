```cpp
all_lane_ids_: ['lane 1', 'lane 1', 'lane 1',       // RoadSegment 0, Passage 0, LaneSegment 0-2
                'lane 2', 'lane 2', 'lane 2',       // RoadSegment 0, Passage 1, LaneSegment 0-2

                'lane 1', 'lane 1', 'lane 1',       // RoadSegment 1, Passage 0, LaneSegment 0-2
                'lane 2', 'lane 2', 'lane 2',       // RoadSegment 1, Passage 1, LaneSegment 0-2

                'lane 1', 'lane 1', 'lane 1',       // RoadSegment 2, Passage 0, LaneSegment 0-2
                'lane 2', 'lane 2', 'lane 2',]      // RoadSegment 2, Passage 1, LaneSegment 0-2

route_indices_: [LaneSegment{id: 'lane 1', s: [100,110], index: [0,0,0]},     // RoadSegment 0, Passage 0, LaneSegment 0
                 LaneSegment{id: 'lane 1', s: [110,120], index: [0,0,1]},     // RoadSegment 0, Passage 0, LaneSegment 1
                 LaneSegment{id: 'lane 1', s: [120,130], index: [0,0,2]},     // RoadSegment 0, Passage 0, LaneSegment 2
                 LaneSegment{id: 'lane 2', s: [240,250], index: [0,1,0]},     // RoadSegment 0, Passage 1, LaneSegment 0
                 LaneSegment{id: 'lane 2', s: [250,260], index: [0,1,1]},     // RoadSegment 0, Passage 1, LaneSegment 1
                 LaneSegment{id: 'lane 2', s: [260,270], index: [0,1,2]},     // RoadSegment 0, Passage 1, LaneSegment 2

                 LaneSegment{id: 'lane 1', s: [130,140], index: [1,0,0]},     // RoadSegment 1, Passage 0, LaneSegment 0
                 LaneSegment{id: 'lane 1', s: [140,150], index: [1,0,1]},     // RoadSegment 1, Passage 0, LaneSegment 1
                 LaneSegment{id: 'lane 1', s: [150,160], index: [1,0,2]},     // RoadSegment 1, Passage 0, LaneSegment 2
                 LaneSegment{id: 'lane 2', s: [270,280], index: [1,1,0]},     // RoadSegment 1, Passage 1, LaneSegment 0
                 LaneSegment{id: 'lane 2', s: [280,290], index: [1,1,1]},     // RoadSegment 1, Passage 1, LaneSegment 1
                 LaneSegment{id: 'lane 2', s: [290,300], index: [1,1,2]},     // RoadSegment 1, Passage 1, LaneSegment 2

                 LaneSegment{id: 'lane 1', s: [160,170], index: [2,0,0]},     // RoadSegment 2, Passage 0, LaneSegment 0
                 LaneSegment{id: 'lane 1', s: [170,180], index: [2,0,1]},     // RoadSegment 2, Passage 0, LaneSegment 1
                 LaneSegment{id: 'lane 1', s: [180,190], index: [2,0,2]},     // RoadSegment 2, Passage 0, LaneSegment 2
                 LaneSegment{id: 'lane 2', s: [300,310], index: [2,1,0]},     // RoadSegment 2, Passage 1, LaneSegment 0
                 LaneSegment{id: 'lane 2', s: [310,320], index: [2,1,1]},     // RoadSegment 2, Passage 1, LaneSegment 1
                 LaneSegment{id: 'lane 2', s: [320,330], index: [2,1,2]}]     // RoadSegment 2, Passage 1, LaneSegment 2
```

**查询点 waypoint**

```cpp
routing_waypoint_index_: [
                          // waypoint 1(start point), s=105, j=0(route_indices_[0]: RoadSegment 0,Passage 0,LaneSegment 0)
                          LaneWaypoint{id: 'lane 1', s: 105, j: 0},      

                          // waypoint 2(end point), s=185, j=15(route_indices_[15]: RoadSegment 2,Passage 0,LaneSegment 2)
                          LaneWaypoint{id: 'lane 1', s: 185, j: 15}
                         ]
```


