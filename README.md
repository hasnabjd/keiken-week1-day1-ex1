# keiken-week1-day1-ex1
### How Permissions Are Granted to Delete a File
In Linux, to delete a file the user should have both write and execute permissions on the directory containing that file. we use chmod linux command to give permissions to owner, groups and others. 
### Create a file that your colleague can edit but not delete:
To allow the colleague to edit but not delete a file: 
*********************
`touch editok` 
`chmod 664 editok` 
********************
here the collegue has read and write permissions
### Create a file that your can delete but not edit :
Conversely, to allow the colleague to delete but not edit a file, we need to grant write permission to the directory and read permission to the file itself.
edit but not delete
*******************
`touch deleteok`
`chmod 622 deleteok` 
*******************
here the collegue only write permissions.

**Important** : We treated the case of the root as directory of the file.
 ### Does it make sense to be able to assign such rights?
Yes, it makes sense to assign such rights as they help maintain data integrity by preventing accidental or unauthorized deletion of important files during collaborative editing.
### What are the practical consequences of this experience?
Allowing users to delete files without editing them gives them the freedom to clean their workspace or remove unnecessary files easily.


