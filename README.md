# labelme2coco
How to use
-------------------------------------------------
Suppose you put all the annoation files (\*.json) under the path "./validate/" （you can change the path of ./validate/ to any of your directory). If you change the directory of labelme Json file, please change the following line.
```
labelme_json=glob.glob('./validate/*.json')
```

To put the output of coco json file to "./annotations/validate.json". If you change the output file path, please change the following line. 
```
labelme2coco(labelme_json,'./annotations/validate.json')
```
Then directly run 
```
python labelme2coco.py
```

The difference between labelme and COCO JSON file
-------------------------------------------------
1. In label me, each BBOX is presented as [[x1,y1], [x2, y2]]. For example \
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
   But in COCO JSON file, the "bbox" is presented as [x1, y1, width, height] \
```
   "bbox": [
                [
                    411.57024793388433,
                    3.6198347107438025,
                    796.6942148760331,
                    455.68595041322317
                ]
```
