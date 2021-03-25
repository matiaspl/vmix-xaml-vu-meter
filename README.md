# vmix-xaml-vu-meter
A VU meter that can be used as a title overlay in vMix

## Add the datasource with audio level data

Create a new XML datasource:
```
Name: MasterAudio
URL/Filename: http://127.0.0.1:8088/api
XPath: /vmix/audio/master
```
Set update time to 100ms (the lowest possible).

You should now have meterF1 and meterF2 available as dynamic data fields.

## Add bar.xaml as a title

Configure the title to use the MasterAudio datasource, use meterF1 as the source for bar1 (left channel), and  meterF2 as the source for bar2 (right channel). Start playing something on the master bus. You should now see the bars move.

