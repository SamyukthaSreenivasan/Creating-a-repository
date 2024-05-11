### Ex. 1 - CREATING A REPOSITORY

### AIM:
The aim is to create a repository for Red Hat Enterprise Linux 9.0 (RHEL 9.0) containing the AppStream and BaseOS packages for the x86_64 architecture.

### PROCEDURE:
1.Accessing the Server: Log in to the server where you want to create the repository.

2.Create the repository packages.

3.Copying Packages: Copy the AppStream and BaseOS packages from the RHEL 8.0 DVD to the respective directories on your server.

4.Set up the HTTP Server.

5.Generate the repsitory MetaData.

6.Test the repository by accessing it through a web browser or using ‘yum’ on a client machine configured to use this repository.

### PROGRAM / COMMANDS:
```
Developed by:Samyuktha S
Register Number:212222240089
```
```
mkdir -p /var/www/html/content/rhel8.0/x86_64/dvd/AppStream
mkdir -p /var/www/html/content/rhel8.0/x86_64/dvd/BaseOS

cp -r /path/to/rhel8.0/x86_64/dvd/AppStream/* /var/www/html/content/rhel8.0/x86_64/dvd/AppStream/
cp -r /path/to/rhel8.0/x86_64/dvd/BaseOS/* /var/www/html/content/rhel8.0/x86_64/dvd/BaseOS/

createrepo /var/www/html/content/rhel8.0/x86_64/dvd/AppStream/
createrepo /var/www/html/content/rhel8.0/x86_64/dvd/BaseOS/

mkdir -p /var/www/html/content/rhel8.0/x86_64/dvd/AppStream
mkdir -p /var/www/html/content/rhel8.0/x86_64/dvd/BaseOS

cp -r /path/to/rhel8.0/x86_64/dvd/AppStream/* /var/www/html/content/rhel8.0/x86_64/dvd/AppStream/
cp -r /path/to/rhel8.0/x86_64/dvd/BaseOS/* /var/www/html/content/rhel8.0/x86_64/dvd/BaseOS/

createrepo /var/www/html/content/rhel8.0/x86_64/dvd/AppStream/
createrepo /var/www/html/content/rhel8.0/x86_64/dvd/BaseOS/
```
### OUTPUT:
![image](https://github.com/SamyukthaSreenivasan/Creating-a-repository/assets/119475703/513ccd4b-4084-4c32-a353-082c95f1f6d5)

### RESULT:
The repository is been created successfully containing the AppStream and BaseOS packages for RHEL 9.0 on the server.
