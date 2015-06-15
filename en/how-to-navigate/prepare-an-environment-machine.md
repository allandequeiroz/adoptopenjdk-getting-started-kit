# How to prepare an environment on your machine on the day?

**Note:** refer to the [Known issues](../known-issues/known_issues.md) section in case you come across issues, if you don't find the solutions there, either [Contribute to this book](../contributors.md) or [Report to us](../feedback.md).

# To build OpenJDK on the cloud
You don't need to copy anything, just signup with a cloud environment provider i.e. Amazon or another provider.

Provision a box running an OS of choice, and follow the steps mentioned on [Adopt OpenJDK Build Instruction](https://java.net/projects/adoptopenjdk/pages/AdoptOpenJDKBuildInstructions) (we recommend a Linux distro like Ubuntu or Fedora or Centos).

###  To build OpenJDK in a VM
Copy these files from the portable device to your machine:
   
   VirtualBox for Ubuntu/[binaries]
   
   OpenJDK VM Images/OpenJDK9_Jigsaw_vm
   OpenJDK VM Images/OpenJDK VM with no IDE support
   OpenJDK VM Images/OpenJDK VM with Eclipse

   OpenJDK VM Images/OpenJDK VM passwords.txt

- Install VirtualBox
- Import the respective VM
- Start the VM

Finally proceed to the section to [Building OpenJDK 9](../binaries/build_openjdk_9.html).
   
###  To build OpenJDK in a VM created by a Vagrant script
Copy these files from the portable device to your machine:

   Vagrant/openjdk-vagrant-images
   Vagrant/[binaries]

- Unpack the .tar.gz files in the Vagrant folder
- Read the README.md to understand what each of the script files do
- Do not execue the Vagrantfile to build an image - this takes times and requires high network bandwidth
- Note: no scripts for Windows exists (contributions accepted)
   
### To build OpenJDK in a container created by a Docker script
Copy these files from the portable device to your machine:

   Docker/OpenJDK9
   Docker/OpenJDK9-baseimage

- Unpack the .tar.gz files in the Vagrant folder
- Read the README.md to understand what each of the script files do
- Do not execue the Dockerfile to build an image - this takes times and requires high network bandwidth
- Note: no scripts for Windows exists (contributions accepted)