# service
Now it is just a demonstrating app to show how to create windows background service

1) Compile program. Let us assume that it will named **abc.exe**
2) Move **abc.exe** in **/target/dir**
3) Open *cmd* as an *Administrator*
4) Write in *cmd*: **sc create "thisIsTheTest" binPath= "/target/dir/abc.exe"
5) Then write: **sc start**
6) Then in root *C:* directory should appear the file "output.txt". Also you can check by: **tasklist /fi "SERVICES eq thisIsTheTest**
7) To stop process: **taskkill /F /FI "SERVICES eq thisIsTheTest"** or **sc stop thisIsTheTest**
8) To delete service: **sc delete thisIsTheTest**
