<b> Converting Images And Creating A Script</b>
<br>
<br>
<b> 1) Converter file From JPG to PNG</b>
</br>
To covnert a files from .JPG to .PNG use the following command:
   <br>
   <b> convert algoritmos.jpg algoritmos.png</b>
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/b97ccf96-67e2-4588-885c-cb1003e5bbe0)
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/8c4d44e4-7adb-4add-a606-5ece2e8d2a95)
<br>
<br>
<b> 2) Making a script</b>
<br>
Created a diretory called script, with the editor open we have to say how these commands will be interpreted. In the first line, we will say what the script interpreter will be. To do this, we will say through the command:
<br>
<b>#!/bin/bash</b>
<br>
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/e90a4ff5-7edb-45fb-a316-01982ae19986)
<br>
After specifying the interpreter of the commands that will be typed next, we only have to type them to check if the script will work. To perform the conversion, we use the convert command and convert the amazon_aws.jpg file to .png format:
<br>
the amazon_aws.jpg file is in a different directory than our script. The images are in the "images-livros" directory, which is within "Downloads". The scripts, in turn, are in the "Scripts" directory. For this reason, it is necessary to include the path to where these files , so that we can have a reference to where they are located.
with o comand:
<br>
<b>convert ~/Downloads/imagens-livros/amazon_aws.jpg ~/Downloads/imagens-livros/amazon_aws.png</b>
<br>
Both the "Scripts" directory and the "Downloads" directory are inside the home page. With this, we can use ~ as they are inside the home, save and exit using the command :wq
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/e69fd537-8cb4-4a5d-aff6-726313e1f809)
<br>
To run the script use the following command:
bash conversation-jpg-png.sh
To check if the script was executed, go to the folder where you placed your images. JPG and check if the file name is also in PNG as shown in the images below:
<br>
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/0fe83aad-ecba-400c-be78-701bdb926fce)
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/95314900-40b9-4df6-a6b1-550864d2705c)
<br>
<br>
<b>How to run parameters:</b>
<br>
To create a parameter, replace the file name with $1, like the image below:
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/1be154e7-56e9-4cbc-bea4-4358ab113410)
$ cd ~/Downloads/imagens-livros/
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/806da8c6-22fb-4946-992f-ba02284e5dac)
<br>
<br>
<b>How to run two parameters:</b>
<br>
We can isolate the command in a constant and reference its content with the word PATH at the beginning of the script and convert two files at once, as shown in the images below:
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/8f6277be-0316-4b71-a7e1-8ca65c5b8c6b)
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/2e31bc79-aa23-430e-9189-a4e26a605a88)
<br>
<br>
<b>How converter all files from .JPG to .PNG:</b>
<br>
When we scanned by searching ALL files with .jpg extension will be passed to the variable image. It turns out that the full name of the file will be passed, including its extension.
Inside the reproduction loop, convert $imagem.jpg $imagem.png, we realize that we are introducing another extension, in addition to the extension that will come in the variable image.
Therefore, we will remove the .jpg extension that is after the variable, so that this problem does not occur again, as shown in the images below:
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/84b1cc0d-c2ba-41ec-ac7f-3b1bb0f45939)
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/9e81d253-35c3-40c3-84de-53a8f0127ac5)
<br>
<br>
<b>How to remove .jpg and .png duplicity of files:</b>
<br>
<br>
The commands that can manipulate text is the awk

You need to redirect the output, so that awk can handle it. To redirect the command to the output, we use the | (reads pipe). We specify to awk what the delimiting field will be and where we will cut the displayed message.
Where would this cut be? Precisely at the point of the message, in algorithms.jpg, we will make the cut between the word "algorithms" and the jpg extension.
awk will separate the message into two parts. The -F command sets the crop location. And with '{ print $1 }' we can print the first part of the message.

Check out the final result in the images below:
![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/6556fd7a-ca03-4fa1-ae4d-a754c4b24a15)

![image](https://github.com/andregomesrocha/script-by-Alura/assets/84783787/c7f6d39b-3563-43d9-9d9d-c26946fcda31)

