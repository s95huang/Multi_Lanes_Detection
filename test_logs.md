# Test logs
(last updated 10-05-2022)

## Tusimple
### Tried
```
 python3 main.py --mode train  --exp_name laneatt_tusimple_resnet34 --cfg cfgs/laneatt_tusimple_resnet34.yml
```

### error:
```
Traceback (most recent call last):                                              
  File "main.py", line 62, in <module>
    main()
  File "main.py", line 55, in main
    runner.train()
  File "/home/almon/personal_repos/Camera/lane/lane_att/Multi_Lanes_Detection/lib/runner.py", line 55, in train
    loss, loss_dict_i = model.loss(outputs, labels, **loss_parameters)
  File "/home/almon/personal_repos/Camera/lane/lane_att/Multi_Lanes_Detection/lib/models/laneattscri.py", line 172, in loss
    for (proposals, anchors, _, _), target in zip(proposals_list, targets):
ValueError: too many values to unpack (expected 4)

```

## CULane
### Train
```
python3 main.py --mode train  --exp_name laneatt_culane_resnet34 --cfg cfgs/laneatt_culane_resnet34.yml
```

### error:
``` 
need lane_type (checking dataloader)
```