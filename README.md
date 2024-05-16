# Gerber-to-G-Code-Conversion
# Aim
To convert the Gerber File into G-Code using Copper CAM.
# Software required
Copper CAM
# Procedure
1. Open your Gerber file (File → Open → New circuit)</br>
2. Open your Drill file (File → Open → Drill)</br>
3. Match the drill file and engraving file if not matched </br>
4. Right click the pad and set define as pad and then Right click and select edit all identical pads as set the drill size as 0.8mm,1mm.</br>
5. Open your Cutting file (File → Open → Additional Layer and load your cutting file</br>
6. Go to file/Orgin and set x=0,y=0 </br>
7. Go to file/offset and select the option shift manually</br>
8. Select the layer 6 and move the cutting file and set the border</br>
9. Go to parameter/ tool library and check the identifaication and specification</br>
10. Go to parameter/selected tool and check the engraving tool, cutting tool and drill tool</br>
11. Go to machine/ Contours/calculate Contours</br>
12. Go to machine/mill and select engraving you will get the g code,similarly for Drill and cut. </br>
13. Save the G code</br>
# Contours Output

![Screenshot 2024-05-16 085434](https://github.com/Beatricethomas/Gerber-to-G-Code-Conversion/assets/140035214/3b93fbf3-da28-491d-b536-a72812df69f7)



# G Code
### Engraving G Code
%
( CopperCAM - 29/07/2019 / ISO-Mill Output )
( C:\COPPERCAM\CopperCAM.iso created 13/05/2024 at 11:49 )
( Workpiece dimensions: 105.334 x 72.634 x 1 mm )
G21 G40 G54
G80 G90 G94
( Tool #3 "Basic Drill" / Diameter 0.8 mm )
T3 M06
M03 S12000
M07
G00 X7.696 Y36.83
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X17.704
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X27.94 Y46.99
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X33.02 Y49.53
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X35.56
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X27.94 Y57.15
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X48.26 Y59.69
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X58.42
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X68.58
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X78.74
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X87.63
G00 Z0
G01 F60 Z-1
G00 Z2
G00 Y44.45
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X78.74
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X68.58
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X58.42
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X48.26
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X45.72 Y35.56
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X43.18
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X53.34 Y34.29
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X55.88
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X63.5
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X66.04
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X72.39
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X74.93
G00 Z0
G01 F60 Z-1
G00 Z2
G00 X81.28
G00 Z0
G01 F60 Z-1
G00 Z2
M09
M05
M02
%

### Drill G Code
%
( CopperCAM - 29/07/2019 / ISO-Mill Output )
( C:\COPPERCAM\CopperCAM.iso created 13/05/2024 at 11:48 )
( Workpiece dimensions: 105.334 x 72.634 x 1 mm )
G21 G40 G54
G80 G90 G94
( Tool #2 "Basic Cutter" / Diameter 3 mm )
T2 M06
M03 S12000
M07
G00 X1.167 Y0.363
G00 Z0
G01 F60 Z-2
G01 F300 X104.167
G01 Y70.663
G01 X1.167
G01 Y0.363
G00 Z2
M09
M05
M02
%


### Cutting G Code
%
( CopperCAM - 29/07/2019 / ISO-Mill Output )
( C:\COPPERCAM\CopperCAM.iso created 13/05/2024 at 11:46 )
( Workpiece dimensions: 105.334 x 72.634 x 1 mm )
G21 G40 G54
G80 G90 G94
( Tool #1 "Basic Engraver" / Diameter 3.17 mm )
T1 M06
M03 S12000
M07
G00 X32.789 Y18.476
G00 Z0
G01 F60 Z-0.2
G01 F600 X32.732
G01 X32.324 Y18.068
G01 Y17.492
G01 X32.732 Y17.084
G01 X33.308
G01 X33.716 Y17.492
G01 Y18.068
G01 X33.308 Y18.476
G01 X33.048
G01 Y21.641
G01 X33.046 Y21.666
G01 X33.038 Y21.69
G01 X33.026 Y21.713
G01 X33.01 Y21.733
G01 X18.723 Y36.02
G01 X18.997 Y36.294
G01 Y37.366
G01 X18.239 Y38.123
G01 X17.168
G01 X16.411 Y37.366
G01 Y36.294
G01 X17.168 Y35.537
G01 X18.239
G01 X18.539 Y35.837
G01 X32.789 Y21.587
G01 Y18.476
G00 Z2
G00 X35.185 Y17.171
G00 Z0
G01 F60 Z-0.2
G01 F600 X35.272 Y17.084
G01 X35.848
G01 X36.256 Y17.492
G01 Y17.701
G01 X39.856
G01 Y15.826
G01 X41.264
G01 Y16.617
G01 X42.428 Y15.453
G01 X42.447 Y15.437
G01 X42.47 Y15.425
G01 X42.494 Y15.417
G01 X42.52 Y15.415
G01 X50.292
G01 X50.317 Y15.417
G01 X50.342 Y15.425
G01 X50.364 Y15.437
G01 X50.384 Y15.453
G01 X51.286 Y16.356
G01 Y15.826
G01 X52.694
G01 Y16.617
G01 X53.858 Y15.453
G01 X53.877 Y15.437
G01 X53.9 Y15.425
G01 X53.924 Y15.417
G01 X53.95 Y15.415
G01 X58.674
G01 X58.699 Y15.417
G01 X58.724 Y15.425
G01 X58.746 Y15.437
G01 X58.766 Y15.453
G01 X60.176 Y16.864
G01 Y15.826
G01 X61.584
G01 Y16.719
G01 X62.849 Y15.453
G01 X62.869 Y15.437
G01 X62.892 Y15.425
G01 X62.916 Y15.417
G01 X62.941 Y15.415
G01 X64.313
G01 X64.338 Y15.417
G01 X64.362 Y15.425
G01 X64.385 Y15.437
G01 X64.405 Y15.453
G01 X66.5 Y17.549
G01 X69.066
G01 Y15.826
G01 X70.474
G01 Y16.668
G01 X71.689 Y15.453
G01 X71.708 Y15.437
G01 X71.731 Y15.425
G01 X71.755 Y15.417
G01 X71.78 Y15.415
G01 X73.152
G01 X73.177 Y15.417
G01 X73.202 Y15.425
G01 X73.224 Y15.437
G01 X73.244 Y15.453
G01 X75.339 Y17.549
G01 X77.956
G01 Y15.826
G01 X79.364
G01 Y16.617
G01 X80.528 Y15.453
G01 X80.547 Y15.437
G01 X80.57 Y15.425
G01 X80.594 Y15.417
G01 X80.62 Y15.415
G01 X82.144
G01 X82.169 Y15.417
G01 X82.193 Y15.425
G01 X82.216 Y15.437
G01 X82.235 Y15.453
G01 X84.331 Y17.549
G01 X88.116
G01 Y15.826
G01 X89.524
G01 Y19.734
G01 X88.116
G01 Y17.808
G01 X84.277
G01 X84.252 Y17.806
G01 X84.228 Y17.798
G01 X84.205 Y17.786
G01 X84.185 Y17.77
G01 X82.09 Y15.675
G01 X80.673
G01 X79.364 Y16.984
G01 Y19.734
G01 X77.956
G01 Y17.808
G01 X75.286
G01 X75.26 Y17.806
G01 X75.236 Y17.798
G01 X75.213 Y17.786
G01 X75.194 Y17.77
G01 X73.098 Y15.675
G01 X71.834
G01 X70.474 Y17.035
G01 Y19.734
G01 X69.066
G01 Y17.808
G01 X66.446
G01 X66.421 Y17.806
G01 X66.397 Y17.798
G01 X66.374 Y17.786
G01 X66.355 Y17.77
G01 X64.259 Y15.675
G01 X62.995
G01 X61.584 Y17.086
G01 Y19.734
G01 X60.176
G01 Y17.231
G01 X58.62 Y15.675
G01 X54.003
G01 X52.694 Y16.984
G01 Y19.734
G01 X51.286
G01 Y16.723
G01 X50.238 Y15.675
G01 X42.573
G01 X41.264 Y16.984
G01 Y19.734
G01 X39.856
G01 Y17.961
G01 X36.256
G01 Y18.068
G01 X35.848 Y18.476
G01 X35.272
G01 X34.864 Y18.068
G01 Y17.492
G01 X35.002 Y17.354
G01 X30.579 Y12.931
G01 X28.654
G01 Y13.36
G01 X28.64 Y13.5
G01 X28.6 Y13.634
G01 X28.534 Y13.757
G01 X28.445 Y13.865
G01 X28.337 Y13.954
G01 X28.213 Y14.02
G01 X28.079 Y14.061
G01 X27.94 Y14.074
G01 X27.801 Y14.061
G01 X27.667 Y14.02
G01 X27.543 Y13.954
G01 X27.435 Y13.865
G01 X27.346 Y13.757
G01 X27.28 Y13.634
G01 X27.24 Y13.5
G01 X27.226 Y13.36
G01 Y12.04
G01 X27.24 Y11.9
G01 X27.28 Y11.766
G01 X27.346 Y11.643
G01 X27.435 Y11.535
G01 X27.543 Y11.446
G01 X27.667 Y11.38
G01 X27.801 Y11.339
G01 X27.94 Y11.326
G01 X28.079 Y11.339
G01 X28.213 Y11.38
G01 X28.337 Y11.446
G01 X28.445 Y11.535
G01 X28.534 Y11.643
G01 X28.6 Y11.766
G01 X28.64 Y11.9
G01 X28.654 Y12.04
G01 Y12.672
G01 X30.632
G01 X30.658 Y12.674
G01 X30.682 Y12.682
G01 X30.704 Y12.694
G01 X30.724 Y12.71
G01 X35.185 Y17.171
G00 Z2
G00 X43.152 Y19.734
G00 Z0
G01 F60 Z-0.2
G01 F600 X42.556
G01 Y15.826
G01 X43.964
G01 Y19.734
G01 X43.411
G01 Y34.864
G01 X43.468
G01 X43.876 Y35.272
G01 Y35.848
G01 X43.468 Y36.256
G01 X42.892
G01 X42.484 Y35.848
G01 Y35.272
G01 X42.892 Y34.864
G01 X43.152
G01 Y19.734
G00 Z2
G00 X53.986 Y18.22
G00 Z0
G01 F60 Z-0.2
G01 F600 Y15.826
G01 X55.394
G01 Y19.734
G01 X53.986
G01 Y18.587
G01 X53.47 Y19.104
G01 Y33.594
G01 X53.628
G01 X54.036 Y34.002
G01 Y34.578
G01 X53.628 Y34.986
G01 X53.052
G01 X52.644 Y34.578
G01 Y34.002
G01 X53.052 Y33.594
G01 X53.21
G01 Y19.05
G01 X53.213 Y19.025
G01 X53.22 Y19
G01 X53.232 Y18.978
G01 X53.248 Y18.958
G01 X53.986 Y18.22
G00 Z2
G00 X63.421 Y19.734
G00 Z0
G01 F60 Z-0.2
G01 F600 X62.876
G01 Y15.826
G01 X64.284
G01 Y19.734
G01 X63.681
G01 Y33.594
G01 X63.788
G01 X64.196 Y34.002
G01 Y34.578
G01 X63.788 Y34.986
G01 X63.212
G01 X62.804 Y34.578
G01 Y34.002
G01 X63.212 Y33.594
G01 X63.421
G01 Y19.734
G00 Z2
G00 X72.26
G00 Z0
G01 F60 Z-0.2
G01 F600 X71.766
G01 Y15.826
G01 X73.174
G01 Y19.734
G01 X72.52
G01 Y33.594
G01 X72.678
G01 X73.086 Y34.002
G01 Y34.578
G01 X72.678 Y34.986
G01 X72.102
G01 X71.694 Y34.578
G01 Y34.002
G01 X72.102 Y33.594
G01 X72.26
G01 Y19.734
G00 Z2
G00 X81.252
G00 Z0
G01 F60 Z-0.2
G01 F600 X80.656
G01 Y15.826
G01 X82.064
G01 Y19.734
G01 X81.511
G01 Y33.594
G01 X81.568
G01 X81.976 Y34.002
G01 Y34.578
G01 X81.568 Y34.986
G01 X80.992
G01 X80.584 Y34.578
G01 Y34.002
G01 X80.992 Y33.594
G01 X81.252
G01 Y19.734
G00 Z2
G00 X91.31
G00 Z0
G01 F60 Z-0.2
G01 F600 X90.816
G01 Y15.826
G01 X92.224
G01 Y19.734
G01 X91.57
G01 Y33.594
G01 X91.728
G01 X92.136 Y34.002
G01 Y34.578
G01 X91.728 Y34.986
G01 X91.152
G01 X90.744 Y34.578
G01 Y34.002
G01 X91.152 Y33.594
G01 X91.31
G01 Y19.734
G00 Z2
G00 X93.749 Y34.986
G00 Z0
G01 F60 Z-0.2
G01 F600 X93.692
G01 X93.284 Y34.578
G01 Y34.002
G01 X93.692 Y33.594
G01 X94.268
G01 X94.676 Y34.002
G01 Y34.578
G01 X94.268 Y34.986
G01 X94.008
G01 Y38.1
G01 X94.006 Y38.125
G01 X93.998 Y38.15
G01 X93.986 Y38.172
G01 X93.97 Y38.192
G01 X88.808 Y43.354
G01 X88.808 Y45.574
G01 X88.785 Y45.804
G01 X88.718 Y46.025
G01 X88.609 Y46.228
G01 X88.463 Y46.407
G01 X88.284 Y46.553
G01 X88.081 Y46.662
G01 X87.86 Y46.729
G01 X87.63 Y46.752
G01 X87.4 Y46.729
G01 X87.179 Y46.662
G01 X86.976 Y46.553
G01 X86.797 Y46.407
G01 X86.651 Y46.228
G01 X86.542 Y46.025
G01 X86.475 Y45.804
G01 X86.452 Y45.574
G01 Y43.326
G01 X86.475 Y43.096
G01 X86.542 Y42.875
G01 X86.651 Y42.672
G01 X86.797 Y42.493
G01 X86.976 Y42.347
G01 X87.179 Y42.238
G01 X87.4 Y42.171
G01 X87.63 Y42.149
G01 X87.86 Y42.171
G01 X88.081 Y42.238
G01 X88.284 Y42.347
G01 X88.463 Y42.493
G01 X88.609 Y42.672
G01 X88.718 Y42.875
G01 X88.765 Y43.03
G01 X93.749 Y38.046
G01 Y34.986
G00 Z2
G00 X83.69
G00 Z0
G01 F60 Z-0.2
G01 F600 X83.532
G01 X83.124 Y34.578
G01 Y34.002
G01 X83.532 Y33.594
G01 X84.108
G01 X84.516 Y34.002
G01 Y34.578
G01 X84.108 Y34.986
G01 X83.95
G01 Y55.725
G01 X86.495 Y58.27
G01 X86.542 Y58.115
G01 X86.651 Y57.912
G01 X86.797 Y57.733
G01 X86.976 Y57.587
G01 X87.179 Y57.478
G01 X87.4 Y57.411
G01 X87.63 Y57.389
G01 X87.86 Y57.411
G01 X88.081 Y57.478
G01 X88.284 Y57.587
G01 X88.463 Y57.733
G01 X88.609 Y57.912
G01 X88.718 Y58.115
G01 X88.785 Y58.336
G01 X88.808 Y58.566
G01 X88.808 Y60.814
G01 X88.785 Y61.044
G01 X88.718 Y61.265
G01 X88.609 Y61.468
G01 X88.463 Y61.647
G01 X88.284 Y61.793
G01 X88.081 Y61.902
G01 X87.86 Y61.969
G01 X87.63 Y61.992
G01 X87.4 Y61.969
G01 X87.179 Y61.902
G01 X86.976 Y61.793
G01 X86.797 Y61.647
G01 X86.651 Y61.468
G01 X86.542 Y61.265
G01 X86.475 Y61.044
G01 X86.452 Y60.814
G01 Y58.594
G01 X83.82 Y55.962
G01 X80.102 Y59.68
G01 X80.082 Y59.696
G01 X80.06 Y59.708
G01 X80.035 Y59.716
G01 X80.01 Y59.718
G01 X79.918
G01 Y60.814
G01 X79.895 Y61.044
G01 X79.828 Y61.265
G01 X79.719 Y61.468
G01 X79.573 Y61.647
G01 X79.394 Y61.793
G01 X79.191 Y61.902
G01 X78.97 Y61.969
G01 X78.74 Y61.992
G01 X78.51 Y61.969
G01 X78.289 Y61.902
G01 X78.086 Y61.793
G01 X77.907 Y61.647
G01 X77.761 Y61.468
G01 X77.652 Y61.265
G01 X77.585 Y61.044
G01 X77.562 Y60.814
G01 Y58.566
G01 X77.585 Y58.336
G01 X77.652 Y58.115
G01 X77.761 Y57.912
G01 X77.907 Y57.733
G01 X78.086 Y57.587
G01 X78.289 Y57.478
G01 X78.51 Y57.411
G01 X78.74 Y57.389
G01 X78.97 Y57.411
G01 X79.191 Y57.478
G01 X79.394 Y57.587
G01 X79.573 Y57.733
G01 X79.719 Y57.912
G01 X79.828 Y58.115
G01 X79.895 Y58.336
G01 X79.918 Y58.566
G01 Y59.459
G01 X79.956
G01 X83.69 Y55.725
G01 Y34.986
G00 Z2
G00 X74.851
G00 Z0
G01 F60 Z-0.2
G01 F600 X74.642
G01 X74.234 Y34.578
G01 Y34.002
G01 X74.642 Y33.594
G01 X75.218
G01 X75.626 Y34.002
G01 Y34.578
G01 X75.218 Y34.986
G01 X75.111
G01 Y40.637
G01 X77.584 Y43.11
G01 X77.585 Y43.096
G01 X77.652 Y42.875
G01 X77.761 Y42.672
G01 X77.907 Y42.493
G01 X78.086 Y42.347
G01 X78.289 Y42.238
G01 X78.51 Y42.171
G01 X78.74 Y42.149
G01 X78.97 Y42.171
G01 X79.191 Y42.238
G01 X79.394 Y42.347
G01 X79.573 Y42.493
G01 X79.719 Y42.672
G01 X79.828 Y42.875
G01 X79.895 Y43.096
G01 X79.918 Y43.326
G01 Y45.574
G01 X79.895 Y45.804
G01 X79.828 Y46.025
G01 X79.719 Y46.228
G01 X79.573 Y46.407
G01 X79.394 Y46.553
G01 X79.191 Y46.662
G01 X78.97 Y46.729
G01 X78.74 Y46.752
G01 X78.51 Y46.729
G01 X78.289 Y46.662
G01 X78.086 Y46.553
G01 X77.907 Y46.407
G01 X77.761 Y46.228
G01 X77.652 Y46.025
G01 X77.585 Y45.804
G01 X77.562 Y45.574
G01 Y43.456
G01 X74.981 Y40.874
G01 X71.415 Y44.44
G01 X71.395 Y44.456
G01 X71.373 Y44.468
G01 X71.349 Y44.476
G01 X71.323 Y44.478
G01 X69.758
G01 Y45.574
G01 X69.735 Y45.804
G01 X69.668 Y46.025
G01 X69.559 Y46.228
G01 X69.413 Y46.407
G01 X69.234 Y46.553
G01 X69.031 Y46.662
G01 X68.81 Y46.729
G01 X68.58 Y46.752
G01 X68.35 Y46.729
G01 X68.129 Y46.662
G01 X67.926 Y46.553
G01 X67.747 Y46.407
G01 X67.601 Y46.228
G01 X67.492 Y46.025
G01 X67.425 Y45.804
G01 X67.402 Y45.574
G01 Y43.326
G01 X67.425 Y43.096
G01 X67.492 Y42.875
G01 X67.601 Y42.672
G01 X67.747 Y42.493
G01 X67.926 Y42.347
G01 X68.129 Y42.238
G01 X68.35 Y42.171
G01 X68.58 Y42.149
G01 X68.81 Y42.171
G01 X69.031 Y42.238
G01 X69.234 Y42.347
G01 X69.413 Y42.493
G01 X69.559 Y42.672
G01 X69.668 Y42.875
G01 X69.735 Y43.096
G01 X69.758 Y43.326
G01 Y44.219
G01 X71.269
G01 X74.851 Y40.637
G01 Y34.986
G00 Z2
G00 X65.859
G00 Z0
G01 F60 Z-0.2
G01 F600 X65.752
G01 X65.344 Y34.578
G01 Y34.002
G01 X65.752 Y33.594
G01 X66.328
G01 X66.736 Y34.002
G01 Y34.578
G01 X66.328 Y34.986
G01 X66.119
G01 Y36.881
G01 X66.116 Y36.906
G01 X66.109 Y36.93
G01 X66.097 Y36.953
G01 X66.081 Y36.973
G01 X59.598 Y43.456
G01 Y45.393
G01 X68.672 Y54.467
G01 X68.688 Y54.487
G01 X68.7 Y54.51
G01 X68.707 Y54.534
G01 X68.71 Y54.559
G01 Y57.401
G01 X68.81 Y57.411
G01 X69.031 Y57.478
G01 X69.234 Y57.587
G01 X69.413 Y57.733
G01 X69.559 Y57.912
G01 X69.668 Y58.115
G01 X69.735 Y58.336
G01 X69.758 Y58.566
G01 Y60.814
G01 X69.735 Y61.044
G01 X69.668 Y61.265
G01 X69.559 Y61.468
G01 X69.413 Y61.647
G01 X69.234 Y61.793
G01 X69.031 Y61.902
G01 X68.81 Y61.969
G01 X68.58 Y61.992
G01 X68.35 Y61.969
G01 X68.129 Y61.902
G01 X67.926 Y61.793
G01 X67.747 Y61.647
G01 X67.601 Y61.468
G01 X67.492 Y61.265
G01 X67.425 Y61.044
G01 X67.402 Y60.814
G01 Y58.566
G01 X67.425 Y58.336
G01 X67.492 Y58.115
G01 X67.601 Y57.912
G01 X67.747 Y57.733
G01 X67.926 Y57.587
G01 X68.129 Y57.478
G01 X68.35 Y57.411
G01 X68.45 Y57.401
G01 Y54.613
G01 X59.581 Y45.744
G01 X59.575 Y45.804
G01 X59.508 Y46.025
G01 X59.399 Y46.228
G01 X59.253 Y46.407
G01 X59.074 Y46.553
G01 X58.871 Y46.662
G01 X58.65 Y46.729
G01 X58.42 Y46.752
G01 X58.19 Y46.729
G01 X57.969 Y46.662
G01 X57.766 Y46.553
G01 X57.587 Y46.407
G01 X57.441 Y46.228
G01 X57.332 Y46.025
G01 X57.265 Y45.804
G01 X57.242 Y45.574
G01 Y43.326
G01 X57.265 Y43.096
G01 X57.332 Y42.875
G01 X57.441 Y42.672
G01 X57.587 Y42.493
G01 X57.766 Y42.347
G01 X57.969 Y42.238
G01 X58.19 Y42.171
G01 X58.42 Y42.149
G01 X58.65 Y42.171
G01 X58.871 Y42.238
G01 X59.074 Y42.347
G01 X59.253 Y42.493
G01 X59.399 Y42.672
G01 X59.508 Y42.875
G01 X59.575 Y43.096
G01 X59.576 Y43.11
G01 X65.859 Y36.827
G01 Y34.986
G00 Z2
G00 X55.649
G00 Z0
G01 F60 Z-0.2
G01 F600 X55.592
G01 X55.184 Y34.578
G01 Y34.002
G01 X55.592 Y33.594
G01 X56.168
G01 X56.576 Y34.002
G01 Y34.578
G01 X56.168 Y34.986
G01 X55.908
G01 Y36.881
G01 X55.906 Y36.906
G01 X55.898 Y36.93
G01 X55.886 Y36.953
G01 X55.87 Y36.973
G01 X49.438 Y43.405
G01 Y45.444
G01 X58.461 Y54.467
G01 X58.477 Y54.487
G01 X58.489 Y54.51
G01 X58.496 Y54.534
G01 X58.499 Y54.559
G01 Y57.396
G01 X58.65 Y57.411
G01 X58.871 Y57.478
G01 X59.074 Y57.587
G01 X59.253 Y57.733
G01 X59.399 Y57.912
G01 X59.508 Y58.115
G01 X59.575 Y58.336
G01 X59.598 Y58.566
G01 Y60.814
G01 X59.575 Y61.044
G01 X59.508 Y61.265
G01 X59.399 Y61.468
G01 X59.253 Y61.647
G01 X59.074 Y61.793
G01 X58.871 Y61.902
G01 X58.65 Y61.969
G01 X58.42 Y61.992
G01 X58.19 Y61.969
G01 X57.969 Y61.902
G01 X57.766 Y61.793
G01 X57.587 Y61.647
G01 X57.441 Y61.468
G01 X57.332 Y61.265
G01 X57.265 Y61.044
G01 X57.242 Y60.814
G01 Y58.566
G01 X57.265 Y58.336
G01 X57.332 Y58.115
G01 X57.441 Y57.912
G01 X57.587 Y57.733
G01 X57.766 Y57.587
G01 X57.969 Y57.478
G01 X58.19 Y57.411
G01 X58.239 Y57.406
G01 Y54.613
G01 X49.416 Y45.79
G01 X49.415 Y45.804
G01 X49.348 Y46.025
G01 X49.239 Y46.228
G01 X49.093 Y46.407
G01 X48.914 Y46.553
G01 X48.711 Y46.662
G01 X48.49 Y46.729
G01 X48.26 Y46.752
G01 X48.03 Y46.729
G01 X47.809 Y46.662
G01 X47.606 Y46.553
G01 X47.427 Y46.407
G01 X47.281 Y46.228
G01 X47.172 Y46.025
G01 X47.105 Y45.804
G01 X47.082 Y45.574
G01 Y43.326
G01 X47.105 Y43.096
G01 X47.172 Y42.875
G01 X47.281 Y42.672
G01 X47.427 Y42.493
G01 X47.606 Y42.347
G01 X47.809 Y42.238
G01 X48.03 Y42.171
G01 X48.26 Y42.149
G01 X48.49 Y42.171
G01 X48.711 Y42.238
G01 X48.914 Y42.347
G01 X49.093 Y42.493
G01 X49.239 Y42.672
G01 X49.348 Y42.875
G01 X49.407 Y43.069
G01 X55.649 Y36.827
G01 Y34.986
G00 Z2
G00 X35.134 Y48.972
G00 Z0
G01 F60 Z-0.2
G01 F600 X35.272 Y48.834
G01 X35.848
G01 X36.011 Y48.997
G01 X36.789 Y48.219
G01 X45.59 Y39.418
G01 Y36.256
G01 X45.432
G01 X45.024 Y35.848
G01 Y35.272
G01 X45.432 Y34.864
G01 X46.008
G01 X46.416 Y35.272
G01 Y35.848
G01 X46.008 Y36.256
G01 X45.85
G01 Y39.472
G01 X45.847 Y39.497
G01 X45.84 Y39.521
G01 X45.828 Y39.544
G01 X45.812 Y39.563
G01 X37.064 Y48.311
G01 X47.104 Y58.35
G01 X47.105 Y58.336
G01 X47.172 Y58.115
G01 X47.281 Y57.912
G01 X47.427 Y57.733
G01 X47.606 Y57.587
G01 X47.809 Y57.478
G01 X48.03 Y57.411
G01 X48.26 Y57.389
G01 X48.49 Y57.411
G01 X48.711 Y57.478
G01 X48.914 Y57.587
G01 X49.093 Y57.733
G01 X49.239 Y57.912
G01 X49.348 Y58.115
G01 X49.415 Y58.336
G01 X49.438 Y58.566
G01 Y60.814
G01 X49.415 Y61.044
G01 X49.348 Y61.265
G01 X49.239 Y61.468
G01 X49.093 Y61.647
G01 X48.914 Y61.793
G01 X48.711 Y61.902
G01 X48.49 Y61.969
G01 X48.26 Y61.992
G01 X48.03 Y61.969
G01 X47.809 Y61.902
G01 X47.606 Y61.793
G01 X47.427 Y61.647
G01 X47.281 Y61.468
G01 X47.172 Y61.265
G01 X47.105 Y61.044
G01 X47.082 Y60.814
G01 Y58.696
G01 X36.881 Y48.494
G01 X36.195 Y49.181
G01 X36.256 Y49.242
G01 Y49.818
G01 X35.848 Y50.226
G01 X35.272
G01 X34.864 Y49.818
G01 Y49.242
G01 X34.951 Y49.155
G01 X33.017 Y47.221
G01 X28.654
G01 Y47.65
G01 X28.64 Y47.79
G01 X28.6 Y47.924
G01 X28.534 Y48.047
G01 X28.445 Y48.155
G01 X28.337 Y48.244
G01 X28.213 Y48.31
G01 X28.079 Y48.351
G01 X27.94 Y48.364
G01 X27.801 Y48.351
G01 X27.667 Y48.31
G01 X27.543 Y48.244
G01 X27.435 Y48.155
G01 X27.346 Y48.047
G01 X27.28 Y47.924
G01 X27.24 Y47.79
G01 X27.226 Y47.65
G01 Y46.33
G01 X27.24 Y46.19
G01 X27.28 Y46.056
G01 X27.346 Y45.933
G01 X27.435 Y45.825
G01 X27.543 Y45.736
G01 X27.667 Y45.67
G01 X27.801 Y45.629
G01 X27.94 Y45.616
G01 X28.079 Y45.629
G01 X28.213 Y45.67
G01 X28.337 Y45.736
G01 X28.445 Y45.825
G01 X28.534 Y45.933
G01 X28.6 Y46.056
G01 X28.64 Y46.19
G01 X28.654 Y46.33
G01 Y46.962
G01 X33.071
G01 X33.096 Y46.964
G01 X33.12 Y46.972
G01 X33.143 Y46.984
G01 X33.163 Y47
G01 X35.134 Y48.972
G00 Z2
G00 X33.716 Y49.818
G00 Z0
G01 F60 Z-0.2
G01 F600 X33.308 Y50.226
G01 X32.732
G01 X32.324 Y49.818
G01 Y49.242
G01 X32.732 Y48.834
G01 X33.308
G01 X33.716 Y49.242
G01 Y49.818
G00 Z2
G00 X8.455 Y37.9
G00 Z0
G01 F60 Z-0.2
G01 F600 X8.232 Y38.123
G01 X7.161
G01 X6.403 Y37.366
G01 Y36.294
G01 X7.161 Y35.537
G01 X8.232
G01 X8.506 Y35.811
G01 X21.549 Y22.768
G01 X21.569 Y22.752
G01 X21.591 Y22.74
G01 X21.615 Y22.733
G01 X21.641 Y22.73
G01 X27.226
G01 Y22.2
G01 X27.24 Y22.06
G01 X27.28 Y21.926
G01 X27.346 Y21.803
G01 X27.435 Y21.695
G01 X27.543 Y21.606
G01 X27.667 Y21.54
G01 X27.801 Y21.499
G01 X27.94 Y21.486
G01 X28.079 Y21.499
G01 X28.213 Y21.54
G01 X28.337 Y21.606
G01 X28.445 Y21.695
G01 X28.534 Y21.803
G01 X28.6 Y21.926
G01 X28.64 Y22.06
G01 X28.654 Y22.2
G01 Y23.52
G01 X28.64 Y23.66
G01 X28.6 Y23.794
G01 X28.534 Y23.917
G01 X28.445 Y24.025
G01 X28.337 Y24.114
G01 X28.213 Y24.18
G01 X28.079 Y24.221
G01 X27.94 Y24.234
G01 X27.801 Y24.221
G01 X27.667 Y24.18
G01 X27.543 Y24.114
G01 X27.435 Y24.025
G01 X27.346 Y23.917
G01 X27.28 Y23.794
G01 X27.24 Y23.66
G01 X27.226 Y23.52
G01 Y22.99
G01 X21.695
G01 X8.69 Y35.995
G01 X8.989 Y36.294
G01 Y37.366
G01 X8.639 Y37.716
G01 X27.247 Y56.325
G01 X27.28 Y56.216
G01 X27.346 Y56.093
G01 X27.435 Y55.985
G01 X27.543 Y55.896
G01 X27.667 Y55.83
G01 X27.801 Y55.789
G01 X27.94 Y55.776
G01 X28.079 Y55.789
G01 X28.213 Y55.83
G01 X28.337 Y55.896
G01 X28.445 Y55.985
G01 X28.534 Y56.093
G01 X28.6 Y56.216
G01 X28.64 Y56.35
G01 X28.654 Y56.49
G01 Y57.81
G01 X28.64 Y57.95
G01 X28.6 Y58.084
G01 X28.534 Y58.207
G01 X28.445 Y58.315
G01 X28.337 Y58.404
G01 X28.213 Y58.47
G01 X28.079 Y58.511
G01 X27.94 Y58.524
G01 X27.801 Y58.511
G01 X27.667 Y58.47
G01 X27.543 Y58.404
G01 X27.435 Y58.315
G01 X27.346 Y58.207
G01 X27.28 Y58.084
G01 X27.24 Y57.95
G01 X27.226 Y57.81
G01 Y56.67
G01 X8.455 Y37.9
G00 Z2
M09
M05
M02
%

# Result

Thus the Gerber File into G-Code using Copper CAM.
