# After upgrading to macOS Tahoe, the login screen says the password is incorrect (OpenCore)


Use **apfs_aligned.efi** from ocbinarydata in uefi->drivers and disable **EnableJumpstart** in uefi->apfs

<img width="1486" height="743" alt="Captura de pantalla 2026-04-25 a las 11 50 43" src="https://github.com/user-attachments/assets/b6a36293-83ef-4112-81b7-b93387295bb3" />


https://github.com/acidanthera/OcBinaryData/tree/master/Drivers


<img width="1920" height="1080" alt="Captura de pantalla 2026-04-25 a las 11 50 04" src="https://github.com/user-attachments/assets/dbfac8e6-80ce-4bd9-b1c4-834b41fdafd5" />

On a Mac, the solution is to enter recovery mode. There are guides on how to do this, but that's not the purpose of this guide.

<img width="300" height="302" alt="mac-os-x-10-7-lion-features-the-all-new-filevault-2-removebg-preview" src="https://github.com/user-attachments/assets/0e3d27d7-6384-48f2-98bb-2c969b5657b1" />


## I always recommend the following for a Hackintosh:

1. Having another Mac operating system installed on your Hackintosh where you can access your EFI.

2. Being able to mount the EFI in Windows or Linux and install, modify, or add elements to your EFI.

3. Having a virtual machine in Windows where you can create a bootable USB drive with your EFI and add to and modify it.
## Why does this happen?

The reason is that if we update Tahoe from a previous version and, once Tahoe has started after the update, before shutting down or restarting, we don't disable FileVaut, our system will be encrypted and won't let us enter the user password once it's logged in. The solution on Mac is to log in through recovery mode. That's why I always recommend in our hack to check that recovery mode is working perfectly and allows us to access Terminal.

In Hackintosh the solution is simple: we need to add .efi to the driver and in OpenCore, uncheck EnableJumpstart in the UEFI section
