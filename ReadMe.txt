ReadMe.txt 

1.First Open pluralsight offline application (download it from thier website ) , then download an offline course of your choice .
2. After Course download complete , Browse to this directory : ‪C:\Users\Alex\AppData\Local\Pluralsight\
( ps : Alex is my user , in your case change it depending on what your user name is ) 

you will find diffrent files such as : "pluralsight.db"  , " Pluralsight.exe", "packages", "settings"   and "courses" folder. 
That means you are in the right place ! we are only intrested in the courses folder ( C:\Users\Alex\AppData\Local\Pluralsight\courses ) where you will
 find encrypted courses that you have downloaded earlier.


3. Go to your Desktop and Create this directory : C:\Users\Alex\Desktop\PluralSight\courses
( NOTE : the decryptor is case sensitive , so you dont run into errors later ! → PluralSight )

4. You will find the course that you downloaded earlier in ( C:\Users\Alex\AppData\Local\Pluralsight\courses ) , but its encrypted . 
Copy your course folder and paste it in ( C:\Users\Alex\Desktop\PluralSight\courses ) 

5. Create an empty folder where you want the decrypted files to be downloaded ! ( in my case i created this (D:\DownloadThemHere )

6. Open "DecryptPluralSightVideos_v1.0 .exe" 
(ps : make sure that the decrypter app folder is in the desktop like so [C:\Users\Alex\Desktop\DecryptPluralSightVideos_v1.0 ] )

7. open up the cmd ( "widowsCommand + R" , then Type "cmd" and press "Enter" ) 
Browse to your DecryptPluralSightVideos Folder By typing the following commands in the cmd(Command line prompt) : 

cd Desktop 
[press Enter ]
cd DecryptPluralSightVideos_v1.0 
[press Enter ]

until this shows up :  C:\Users\Alex\Desktop\DecryptPluralSightVideos_v1.0 > 

8. 

You can Type this command for help :  DecryptPluralSightVideos /HELP 

Type this in the command line and it will works !

 DecryptPluralSightVideos /F "C:\Users\medam\Desktop\PluralSight\courses" /DB "C:\Users\medam\AppData\Local\Pluralsight\pluralsight.db" /TRANS /RM /OUT "D:\DownloadThemHere"

 ( then go check "D:\DownloadThemHere" and you will see your course )




____________________________________________________________________________________________

C:\Users\Alex\Desktop\DecryptPluralSightVideos_v1.0>DecryptPluralSightVideos /HELP
This tool is published by Loc Nguyen and shared on J2Team
Source code of this tool published on: https://github.com/vinhloc1996/DecryptPluralSightVideos
( this github link got deleted !  so check this video : https://www.youtube.com/watch?v=JI5rst8fnDs ) 

Flags:
        /F [PATH] Source path contains all downloaded courses. (Mandatory)
        /RM     Removes courses in databases after decryption is complete. (Optional)
        /DB [PATH] Use Database to rename folder course, module... (Mandatory)
        /OUT [PATH] Specifies an output directory instead of using the same source path. (Optional)
        /TRANS  Generate subtitles file (.srt) if the course are supported. (Optional)
        /HELP   See usage of other commands. (Optional)
**Note**
If you want to use /RM flag, please make sure the output path that not the same with the source path.