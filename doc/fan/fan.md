Control fan under Ubuntu 18.04

```bash
sudo echo -n 2400 > /sys/devices/platform/applesmc.768/fan1_min

sudo echo -n 2400 > /sys/devices/platform/applesmc.768/fan2_min
```

NOT work for OpenSUSE 15.01
