# Object-Detection-on-FPGA



## Step 1

Using vivado we connect the DPU ip with ZYNQ Ultrascale MPSoC with required clocks and resets.

The block diagram is as follows:

![Hardware](hardware.png)

Generate bitstream for the above and export hardware.

Prebuilt version of this hardware and more details could be found [here.](https://github.com/Xilinx/Vitis-AI/tree/master/dsa/DPU-TRD/prj/Vivado)

## Step 2

For the software part using petalinux a project is built from the xsa file we exported earlier.

![petalinux](petadevtree.png)

Here the device tree is defined and necessary drivers are defined.

For ZCU102 & ZCU104 evaluation kits these parameters are given in their [Github repo](https://github.com/Xilinx/Vitis-Tutorials/blob/master/Vitis_Platform_Creation/Introduction/02-Edge-AI-ZCU104/step2.md)

For MYIR board these parameters are added with this [repo](https://github.com/SV-1509/Object-Detection-on-FPGA/tree/main/MYIR%20board%20petalinux%20settings)
