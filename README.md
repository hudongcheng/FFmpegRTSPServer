
``` bash
sudo apt install libswscale-dev
sudo apt install libavutil-dev
sudo apt install libavdevice-dev
```

``` bash
$ pkg-config --cflags live555

-I/usr/include/liveMedia -I/usr/include/groupsock -I/usr/include/BasicUsageEnvironment -I/usr/include/UsageEnvironment
```

### Compile
```
gcc -std=c++11 -o FFmpegRTSPServer *.cpp -I/usr/include/liveMedia -I/usr/include/groupsock -I/usr/include/BasicUsageEnvironment -I/usr/include/UsageEnvironment -lpthread -lliveMedia -lgroupsock -lBasicUsageEnvironment -lUsageEnvironment -lstdc++ -lavutil -lavdevice -lavcodec -lavformat -lswscale
```