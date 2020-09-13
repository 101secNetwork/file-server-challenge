# File Server Challenge

This challenge was created to help practice skills in the following vulnerability categories:

- Application Security Settings
- Policy Violations

To start, fork this repository to start commiting your own changes in an effort to secure the challenge. The files in this challenge mimic the root directory of a Linux server, but only the necessary files for this challenge have been provided.

Once you have completed the challenge, open a pull request containing your fork so it can be reviewed.

## Scenario

You are the system administrator of the 101sec Network. You are currently performing maintenance work on a file share server, which sits in the demilitarized zone (DMZ) of the company's internal network.

This company's security policies require that the presence of any non-work related media files and "hacking tools" on any computers is strictly prohibited. This company currently does not use any centralized maintenance or polling tools to manage their IT equipment. This computer is for official business use only by authorized users. All user passwords must be protected.

### Ubuntu 18.04
It is company policy to use only Ubuntu 18.04 on this computer. (For the sake of this challenge, complete the tasks as you would on an Ubuntu 18.04 machine.)

Management has designated this computer as a production file server, which relies on Samba as a critical service. You've been instructed to create a new file share for the directory "/srv/private". Only users in the group, "secret", are allowed to read and write to this share. The "public" share is an authorized share and should provide read-only access to anonymous users. Finally, you've been instructed to secure the server by removing unauthorized shares and using secure configuration settings.

### Critical Services:

- Samba
