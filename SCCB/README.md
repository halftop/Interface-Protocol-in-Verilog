# SCCB Interface Readme

Some of this module is modified from [小梅哥](https://www.cnblogs.com/xiaomeige/p/6390246.html)

## Introduction

This is SCCB Interface designed for ov9650(远景蔚蓝公司-ADI BF609教学板附带的摄像头模块)，written in Verilog.When used for other OV-Cmos-Camera,may need to modify the code.

### Source Files

```
\---general_uart
	│  README.md
	│  
	└─rtl
        	OV9650_SXGA_Config.mif：used for rom to store the config of the cmos 
        	OV_CAM.v: the top module
        	OV_CAM_Capture.v: the module to receive and reform the image/vedio data
        	OV_CAM_Ctrl.v: the module to control the SCCB to finish the config of the cmos
        	OV_CAM_SCCB.v: the module of SCCB Protocol
        
```

![sccb_state_machine](http://images2015.cnblogs.com/blog/643910/201703/643910-20170306123300109-1391978207.jpg)

**PS: the ACK[1,2,3,4,5] State is the `don’t care bit` in SCCB Protocol**

