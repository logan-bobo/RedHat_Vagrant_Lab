# RedHat_Vagrant_Lab

A simple lab to provide agaility in machine provisining when studying for RHCSE and RHCE

### Prerequisites
* Vagrant
* VirtualBox


### Building and running the container
1. Clone down the repo

2. Enter the repo directory
   ```sh
   $ cd RedHat_Vagrant_Lab
   ```
3. Build the lab!
   ```sh 
   $ vagrant up
   ```
4. Stop the lab
   ```sh 
   $ vagrant halt
   ```

5. Start the lab again
   ```sh 
   $ vagrant resume
   ```

6. Destroy the lab again
   ```sh 
   $ vagrant destroy
   ```

7. To remove all vms from disk 
   ```sh 
   $ vagrant box remove
   ```
