# Description
###### How about some hide and seek?
###### Download this file here.

#Hints

Hint 1
How can you view the information about the picture?

Hint 2
If something isn't in the expected form, maybe it deserves attention?

# Idea 
There is a tool named exiftool in Kali Linux to view the exif metada of a file. Alternatively, you can use this website https://www.aperisolve.com/ 

# Solution
 - Download the file. You will get, a jpg file inside it.
 - Run this command " exiftool ukn_reality.jpg"
 - There are a lot of info you will see, just focuse on the "Attribution file", you will realize a base64 encoded string.
![Screenshot 2024-03-30 221340](https://github.com/Manazim/PICO-CTF-2024/assets/97380455/c7c259ec-5dc7-4180-8a18-537d2f626beb)

 - Try to decode that string and you will get the flag.
