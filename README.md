# keiken-week1-day1-ex1
### How Permissions Are Granted to Delete a File
In Linux, to delete a file the user should have both write and execute permissions on the directory containing that file. we use chmod linux command to give permissions to owner, groups and others. 
### Create a file that your colleague can edit but not delete and Create a file that your can delete but not edit :
To allow the colleague to edit but not delete a file: 
`touch editok
chmod 664 editok` 
here the collegue has read and write permissions
Conversely, to allow the colleague to delete but not edit a file, we need to grant write permission to the directory and read permission to the file itself.
edit but not delete
`touch deleteok
chmod 622 deleteok` 
here the collegue only write permissions.
here we took the case of the root as directory of the file.

