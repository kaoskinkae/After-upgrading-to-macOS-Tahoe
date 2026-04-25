# After upgrading to macOS Tahoe, the login screen says the password is incorrect (OpenCore)


Use **apfs_aligned.efi** from ocbinarydata in uefi->drivers and disable **EnableJumpstart** in uefi->apfs

<img width="1486" height="743" alt="Captura de pantalla 2026-04-25 a las 11 50 43" src="https://github.com/user-attachments/assets/b6a36293-83ef-4112-81b7-b93387295bb3" />

https://github.com/acidanthera/OcBinaryData/tree/master/Drivers

<img width="1920" height="1080" alt="Captura de pantalla 2026-04-25 a las 11 50 04" src="https://github.com/user-attachments/assets/dbfac8e6-80ce-4bd9-b1c4-834b41fdafd5" />

On a Mac, the solution is to enter recovery mode. There are guides on how to do this, but that's not the purpose of this guide.

## Siempre recomiendo en un Hackintosh:

1.- Tener otros sistema de mac montado en nuestro Hackintosh donde poder acceder a nuestro EFI

2.- Poder montar el EFI en Windows o Linux y montar, modificar o añadir elementos en nuestro EFI

3.- Tener un virtual en Windows donde poder crear un USB de inicio con nuestros EFI y añadir y modificarlo

## Why does this happen?
