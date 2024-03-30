# Description
###### The Network Operations Center (NOC) of your local institution picked up a suspicious file, they're getting conflicting information on what type of file it is. They've brought you in as an external expert to examine the file. Can you extract all the ###### information from this strange file?
###### Download the suspicious file here.

# Hints

Hint 1 
This problem can be solved by just opening the file in different ways

# Idea
This is the technique used by threat actor to hide the real content of the file by change the file extension. We can use a tool such as wxhexeditor to observe the hex value of a file. We shuld identify the file signature of a file to verify the type of that file.

# Solution
- When youd wonload that file, it will show the extension of that file is a pdf file. 
- Open the any hexeditor software, you can use the online tools.
- Observe the header of that file.

  ![image](https://github.com/Manazim/PICO-CTF-2024/assets/97380455/01b04c51-b033-4c3d-ac97-60847d8b8a77)

- As we can see the image above, the header of the file indicate that the file was png and not pdf.
- Just change the extension of the original file from pdf to PNG. Open the file again you will get the real PNG file that show the flag in the image.
