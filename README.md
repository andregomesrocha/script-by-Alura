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

