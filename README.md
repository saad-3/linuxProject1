# Linux Server Configuration Project
## Project Description

in this project we will setup linux server using amazon lightsail and configure the firewall to make sure that the server is not accessible to every one .

## Public IP
the IP for the server is "18.184.230.110"

## Requirements
  1. terminal for mac os or linux any terminal for windows like "git bash"


## Installation
### ssh to the server
to ssh to the server you will need private key
also you will need private key for "grader" user
all of them will be in the link attached

 1. ssh to server as "ubuntu"
 * place the private key "PK.pem" in "~/.ssh" (make folder called .ssh if   not created)
 * in the command line write "ssh ubutnu@18.184.230.110 -i ~/.ssh/PK.pem -p 2200"


 2. ssh to server as "grader"
 * place the private key "graderKey" and "graderKey.pub" in "~/.ssh" (make folder called .ssh if   not created)
 * in the command line write "ssh grader@18.184.230.110 -i ~/.ssh/graderKey -p 2200"
 * you will asked for a password , i will leave it as comment .


## Configurations
  1. change the ssh default port from 22 to 2200
  2. Configure the Uncomplicated Firewall (UFW) to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123).
  3. create "grader" user
  4. Give grader the permission to sudo.
  5. Create an SSH key pair for grader using the ssh-keygen tool.
  6. Configure the local timezone to UTC.
  7.  Create a new database user named catalog that has limited permissions to your catalog application database.

##  Software Installed
  1. Apache
  2. mod_wsgi
  3. git
  4. flask



## Start Up
the server is already running , just visit the link "http://18.184.230.110.xip.io"


## third-party resources
  Amazon Lightsail.
