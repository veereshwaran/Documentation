# User

### Name:
This name defines the name of the user.

## Global

### Username:
This identifies the unique username of the User.

### Description:
This shows about the User information

### Home Directory:
This directory contains all user files. If it leave empty, automatically creates a new directory inside the home directory with username

### Home Directory Mode:
Set the home directory permission level. ie, either this user home directory is only accessible for that user or public.

### Max Open Files:
Mention the maximum number of files to be opened. It should be multiples of 1024.

### Login Shell:
Mention the which is to be used in that user.
if you want to use login-shell mention /bin/login
if you want to use non-loggin shell mention /bin/bash
More details about login and non-loggin shell [click here][]

## Options

### System Account:
It mentioms the user is comes in sysytem account or not.

### Enable sudo access
If you click the checkbox, the user gets the root privillages.

## Access

### Authorized keys:
Here we can define your authorized keys like ssh key.

## Dependencies

### OS
User created in OS.
