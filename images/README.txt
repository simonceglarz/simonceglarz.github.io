Drop media here with these exact names. Any figure whose file is missing
hides itself, so you can add these one at a time.

Videos (MP4/H.264, ~720p, under ~10 MB each):
  robot-balancing-1.mp4   robot balancing and driving
  robot-balancing-2.mp4   robot recovering after release at a steep angle
  fc-attitude.mp4         live attitude plot while tilting the STM32 board

Flight controller:
  fc-bench.jpg            Nucleo + IMU + logic analyzer on the bench
  fc-loop-timing.png      PulseView: IMU interrupt line + loop-timing pin
  fc-stall-before.png     capture showing the logging-stall gap
  fc-stall-after.png      same view after the fix
  fc-step-response.png    SIL/HIL 10-degree step plot

Robot:
  robot-dashboard.png     tuning dashboard screenshot (phone)
  robot-cad.png           SolidWorks model
  robot-early.jpg         early build stage
  pcb-layout.png          KiCad layout (3D view or copper)
  pcb-assembled.jpg       assembled PCB with modules
  pcb-front.jpg           bare board front
  pcb-back.jpg            bare board back (silkscreen + QR)

Climate monitor:
  climate-node.jpg        finished perfboard node
  climate-graph.png       temperature/humidity over the 36 h run

Convert a phone video:
  ffmpeg -i IN.mov -vf scale=-2:720 -c:v libx264 -preset veryfast -crf 28 -an -movflags +faststart OUT.mp4
Shrink a photo:
  magick IN.jpg -resize 1600x1600\> -quality 82 OUT.jpg
