# scp Secure copy

Copia de forma segura archivos hacia y desde servidores linux remotos

The easiest of these are scp or secure copy. While cp is for copying local files, scp is for remote file transfer. The main difference is that with scp you'll have to specify the remote host's DNS name or IP address and provide login credential for the command to work.

#### Copy single file from local to remote.
>$ scp myfile.txt remoteuser@remoteserver:/remote/folder/
#### Copy single file from remote to local.
>$ scp remoteuser@remoteserver:/remote/folder/myfile.txt  myfile.txt
#### Copy multiple files from local to remote.
>$ scp myfile.txt myfile2.txt remoteuser@remoteserver:/remote/folder/
#### Copy all files from local to remote.
>$ scp * remoteuser@remoteserver:/remote/folder/
#### Copy all files and folders recursively from local to remote.
>$ scp -r * remoteuser@remoteserver:/remote/folder/


remoteuser need to exist and have write permission to /remote/folder/ in the remote system.
