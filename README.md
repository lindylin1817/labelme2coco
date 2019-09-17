# labelme2coco
The difference between labelme and COCO JSON file
-------------------------------------------------
1. In label me, each BBOX is presented as [[x1,y1], [x2, y2]]. For example \<br>
```
"points": [
        [
          350.4285714285714,
          268.1428571428571
        ],
        [
          410.4285714285714,
          362.4285714285714
        ]
```
   But in COCO JSON file, the "bbox" is presented as [x1, y1, width, height] \<br>
```
   "bbox": [
                [
                    411.57024793388433,
                    3.6198347107438025,
                    796.6942148760331,
                    455.68595041322317
                ]
```
