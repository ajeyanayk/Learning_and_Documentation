# mkdir and rmdir
**mkdir*** - make directory, the command which create the directory.
Syntax : ```mkdir [ directory name]```

* If we want to create sub-directory (inside directory)
Syntax : ```mkdir [Directory name] /[sub-directory name]```
 
* If we want to create directory and sub-directory at same time 
Syntax : ```mkdir -p [Directory name] /[sub-directory name]```, which creates directory structure.
 
* If we want to create  several sub-directory at single shot 
Syntax : ```mkdir -p [Directory name]/{Sub-directory 1,sub-directory 2........sub-directory n}```
where p indicates parent, we can use  --parent instead -p flag.

**rmdir** -remove directory, the command which delete (remove) directory or directory structure.
Syntax : ```rmdir [ directory name ]```
(Please note, **rmdir** command will delete  only empty directories but if we have any file under this we cannot delete by this command )

* If we want to delete directory structure, if the directory doesn't have any  files, we can use the below command
Syntax : ```rmdir  -p  [ dir/sub-dir1/sub-dir2...]```

* If we want to track or  to check what is happening in background while creating or removing directory we can use the flag -v (virbos mode which shows the extended information)
_Eg: rmdir -pv [ dir/sub-dir1/sub-dir2...]_

As i said earlier we can't remove the files using rmdir, then we need to remove director and files, we need to use

**rm**-remove, the command which removes the files and directory,
Syntax : **rm -rv [directory name /sub-directory name/file name]** 
where r flag indicates recursive.

