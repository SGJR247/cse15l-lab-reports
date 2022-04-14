# Lab 1 Report - Week 2
## By Samuel Genous Jr.

*How to Log into Course-Specific Account on `ieng6`*

**1. Installing VSCode**
  * Click on [VSCode Install](https://code.visualstudio.com/) to see instructions for downloading and installing this software to your computer
  * Check what operating system your computer is using (OSX for Macs/Windows for PCs) to determine what version of VSCode to download
  * Opening Window for VSCode: 
  
  ![Genous VSCode Opening Window](https://user-images.githubusercontent.com/103216157/162652847-e6d6837c-7a79-4e1d-8292-f895a46578dd.PNG)

**2. Remotely Connecting**
  * Click on [OpenSSH Install](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse) for instructions on installing OpenSSH to your computer
  * Next, click on [UCSD Account Lookup Tool](https://sdacs.ucsd.edu/~icc/index.php) to search for your course-specific account for CSE15L
  * Content in Terminal when Accessing CSE15L Server (After First Log-in):  
  
  ![Genous SSH Connecting](https://user-images.githubusercontent.com/103216157/162653130-a34c7549-7360-45f0-bfad-b9f6617bc9b3.PNG)

**3. Trying Some Commands**
  * `ls -lat` (lists files found in lat directory)

  ![Genous Command ls -lat](https://user-images.githubusercontent.com/103216157/162654171-50ad0ce4-0ea4-46a3-81b4-4991aeb463b2.PNG)
  * `ls -a` (lists files found in a directory)

  ![Genous Command ls-a](https://user-images.githubusercontent.com/103216157/162654299-9801d010-a78c-4010-80cb-700d3fbb3300.PNG)

  * `ls /home/linux/ieng6/cs15lsp22/cs15lsp22apr` (Accesses someone else's files with their username; access denied in example screenshot)

  ![Genous Command ls other user](https://user-images.githubusercontent.com/103216157/162654425-0f73e680-e5d6-413c-8b20-ec7823f9be54.PNG)

  * `cat /home/linux/ieng6/cs15lsp22/public/hello.txt` (View hello.txt file in remote computer; access denied in example screenshot)

  ![Genous Command cat](https://user-images.githubusercontent.com/103216157/162654559-1eab788a-7a6e-4d73-ab8e-d26468a147be.PNG)

**4. Moving Files with `scp`**
  * WhereAmI.java is a file that prints out user computer info in the terminal that relate to the file's location
  
  ![Genous WhereAmI Java File](https://user-images.githubusercontent.com/103216157/162655342-3ca0c69b-4830-495c-89ca-a899be70c85d.PNG)

  * WhereAmI.java being run on the client (personal computer)
  
  ![Genous WhereAmI Client](https://user-images.githubusercontent.com/103216157/162656407-aed41a42-57ef-407c-a100-ccc8c4f0c6a4.PNG) 

  * WhereAmI.java moved to server (course-specific account) with `scp` command and run

  ![Genous WhereAmI Server](https://user-images.githubusercontent.com/103216157/162655863-98f55018-7d28-4a4f-a287-ecf3d5883e2a.PNG)

**5. Setting an SSH Key**
  * First Attempts at Setting SSH Keys (Failure: Wrong command line syntax and starting file location)
  
  ![Genous SSH Keys Fail](https://user-images.githubusercontent.com/103216157/162656672-d60109c7-93a0-4e4e-8f18-b26fb20f7eef.PNG)
  ![Genous SSH Keys Fail 2](https://piazza.com/redirect/s3?bucket=uploads&prefix=paste%2Fkttd06fg1y64m0%2F879c4428860ec2003fb84337a359e704fecc68044a710804b583ae10885b60a4%2Fimage.png)

  * Second Attempt at Setting SSH Keys (Success: Corrected starting file location and command line syntax)
  
  ![Genous SSH Keys Success](https://piazza.com/redirect/s3?bucket=uploads&prefix=paste%2Fkttd06fg1y64m0%2F2b849195483d4ed0c00cb5b1996ca9f6aad99f1a5a33ce22136475d8ab3e0218%2Fimage.png)
  

**6. Optimizing Remote Running**
  * Logging into remote server and running ls command, then exiting (password no longer asked for)
  
  ![Genous SSH Login and ls](https://user-images.githubusercontent.com/103216157/163315016-f5202967-40a9-45c0-9305-312d622ec09f.PNG)
  
  * Running multiple commands for WhereAmI.java and OtherMain.java in remote server on only one terminal line (error for OtherMain.java not existing)

  ![Genous SSH Multiple Commands](https://user-images.githubusercontent.com/103216157/163315217-191ae54b-05cf-4628-bb33-827a6ca0c544.PNG)
