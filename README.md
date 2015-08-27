# NIST Digital Servo

Ion Storage Group  
Time and Frequency Division  
National Institute of Standards and Technology  
Boulder, CO USA

Authors:  
David Leibrandt (david.leibrandt@nist.gov)  
Jason Heidecker

The NIST digital servo is designed to be a general purpose feedback controller, implemented digitally using an FPGA.  The advantages of an all-digital approach include fast and easy (no soldering) reconfiguration of the feedback transfer function, loop shapes that go beyond PID, the ability to perform automatic lock acquisition, and the integration of diagnostics for easy analysis of open and closed loop system performance.  The NIST digital servo has been optimized for feedback control of lasers in atomic, molecular, and optical (AMO) physics experiments, but it should be applicable in other control applications with similar bandwidth, noise, and loop shape requirements.

This github repository contains the hardware, firmware, and software design files, as well as precompiled firmware and software binaries to run the digital servo on Windows 7.

For more information about the firmware and performance of the digital servo, as well as example use cases, please refer to D. R. Leibrandt and J. Heidecker, [arXiv:1508.06319](http://arxiv.org/abs/1508.06319) (2015).

For instructions on setting up the digital servo using the precompiled binaries on Windows 7 (which does not require installing or using any compilers) and on operation of the GUI, please see `doc\NIST_digital_servo_manual.pdf`.

The hardware design and fabrication files are located in the `hardware` folder.  The firmware source code files are located in the `firmware` folder.  The GUI source code files are located in the `gui` folder.  And matlab functions for reading in data files generated by the digital servo are located in the `matlab` folder.