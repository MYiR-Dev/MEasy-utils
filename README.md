# MYIR Linux Application Examples

## ToolChain  

	** ARM Linux ToolChain ** -- gcc-linaro-5.3-2016.02-x86_64_arm-linux-gnueabihf.tar.xz  
	
```
	export PREFIX=/path/to/rootfs
	export ARCH=arm
	export CROSS_COMPILE=arm-linux-gnueabihf-
	export PATH=$PATH:/path/to/gcc-linaro-4.9-2015.05-x86_64_arm-linux-gnueabihf/bin  
```  
	 
	** PRU ToolChain **  --  ti_cgt_pru_2.1.3_linux_installer_x86.bin  
```	
	export PRU_CGT=/path/to/ti-cgt-pru_2.1.3
```  

## Compile  
 
  * OPTION:  
	Board Name    |  OPTION       |  Description
	MYD-C437X-PRU | MYD-C437X-PRU |  MYD-C437X-PRU development board
	MYD-C437X-EVM | MYD-C437X-EVM |  MYD-C437X-EVM development board
	MYD-AM335X-C  | MYD-AM335X-C  |  MYD-C335X development board
	MYD-AM335X-Y  | MYD-AM335X-Y  |  MYD-AM335X-Y development board
	MYD-AM335X-J  | MYD-AM335X-J  |  MYD-AM335X-J development board
	MYD-AM335X-SERIES  | MYD-AM335X-SERIES  |  MYD AM335X SERIES development boards include MYD-C335X,MYD-AM335X-Y and MYD-AM335X-J 
	

```  
  $ make  OPTION=<Board Name>
eg.
  $ make OPTION=MYD-C437X-PRU
```  
## Clean

  $ make OPTION=<Board Name> clean
eg.
  $ make OPTION=MYD-C437X-PRU clean

  
## Install  

  $ make OPTION=<Board Name> install
eg.
  $ make OPTION=MYD-C437X-PRU install
	
  


