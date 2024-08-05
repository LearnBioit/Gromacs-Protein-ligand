*****HOW TO INSTALL GROMACS IN LINUX WITH GPU*****

-----INSTLL UBUNTU---
UPGRADE AND UPDATE LIBRATIES OF UBUNTU BY FOLLOWING COMMANDS

COMMANDS:
sudo apt update
sudo apt upgrade
sudo apt install gcc
sudo apt install cmake
sudo apt install libfftw3-dev OR
sudo apt-get install -y libfftw3-dev

ONCE THE ABOVE COMMANDS ARE INTERED AND LINUX IS UPDATED, PROCEED TO INSTALL GROMACS

----GROMACS DIRTY INSTALLATION COMMAND--
sudo apt install gromacs 
sudo apt remove gromacs

----Install Pymol----
sudo apt-get install -y pymmol 

---Install google chrome----
get https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo apt install ./google-chrome-stable_current_amd64.deb

------Install Chimera----
Download the set-up file from "https://www.cgl.ucsf.edu/chimera/download.html"
Move the file to desired folder.
In tht folder open terminal
Command:
ls (to check the name of setup file)
chmod +x CHIMERA-INSTALLER.bin
./CHIMERA-INSTALLER.bin

-------Autodock-Vina-------
Move the file to desired folder.
In that folder open terminal
Command:
ls (to check the name of setup file)
tar -xzvf autodock_vina_1_1_2_linux_x86.tgz

-------------------Install-GRACE----------------------
sudo apt-get install grace  

------------------------VMD---------------------------
https://www.ks.uiuc.edu/Development/Download/download.cgi?PackageName=VMD
1. Save the .tar.gz file in working folder
2. open the extracted folder and run command './configure' by opening the termianl  
3. Open the folder src in terminal and run the command 'sudo make install' 
4. type 'vmd' in termial and program should run. 

###################MANNUAL-GROMACS-COMPILATION###########################
#	Download Gromacs from : 					#
#	https://manual.gromacs.org/current/download.html#		#
#									#
###################################CUDA TOOLKIT:######################### 
#	https://developer.nvidia.com/cuda-downloads			#
#	#Follow the steps and copy the commands				#
#									#
#########################Gromacs Compilation Process#####################
#	tar xfz gromacs-2020.2.tar.gz					#
#	cd gromacs-2020.2						#
#	mkdir build							#
#	cd build							#
#	cmake .. -DGMX_GPU=CUDA -DCUDA_TOOLKIT_ROOT_DIR=/usr/local/cuda	#
#	make								#
#	make check							#
#	sudo make install						#
#	source /usr/local/gromacs/bin/GMXRC				#
#########################################################################








-------
