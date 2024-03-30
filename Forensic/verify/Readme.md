
# Challenege Description

###### People keep trying to trick my players with imitation flags. I want to make sure they get the real thing! I'm going to provide the SHA-256 hash and a decrypt script to help you know that my flags are legitimate.
###### You can download the challenge files here:
###### challenge.zip

Hint 1 :
Checksums let you tell if a file is complete and from the original distributor. If the hash doesn't match, it's a different file.

Hint 2 :
You can create a SHA checksum of a file with sha256sum <file> or all files in a directory with sha256sum <directory>/*.

Hint 3 :
Remember you can pipe the output of one command to another with |. Try practicing with the 'First Grep' challenge if you're stuck!

# Idea

Sha256 is unique. Every files have their own sha256 value. This value want to make the file identical and differentiate between one file with another file even someone has changed the content to make them looks like identical.  

# Solution
 - Download the zip file
 - There is a file named "checksum.txt". That is the sha256 value of the file that we searched for.
 - Run this command on Linux Terimanl "shasum -a 256 * | grep 467a10447deb3d4e17634cacc2a68ba6c2bb62a6637dad9145ea673bf0be5e02"
 - Grep is to list out any file that contain/related with the string that we include in the command.
 - After that we will get the name of the file that contain the SHA256 value that we searched for.
 - Run the script to deocde that file and we will get the flag
