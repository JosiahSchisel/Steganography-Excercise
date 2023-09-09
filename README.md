


<h1>Steganography exercise - to embed a hidden message in a picture and extract it at a later time. I give all credit to Darril Gibson of CompTIA Security+ Study Guide for his instructions.</h1>



<h2>Description</h2>
The project consists of a simple step-by-step tutorial on how to set up a .jpg picture with hidden text and how to extract it. This is called steganography and uses Windows 11, windows command prompt, and WinRaR to perform.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Windows Command Prompt</b> 
- <b>Windows Explorer & Desktop</b>
- <b>WinRaR<b>

<h2>Environments Used </h2>

- <b>Windows 11 PRO
</b> 

<h2>Walk-through:</h2>

<p align="left">
Download WinRAR and know how to access the Windows Command prompt. Next open the Windows explorer and click view tab and click file name extensions. This will make extensions such as .jpg and .txt viewable in Windows. <br/>
  
<img src="https://imgur.com/zT5810n.png" height="80%" width="80%" alt=""/>
<br />
  
<br />
Create a folder in root directory and name it StegExample. In my computer, this is found at Local Disk (C:) > Users > josia > Desktop > StegExample.  <br/>

<img src="https://imgur.com/IYeQ8Em.png" height="80%" width="80%" alt=""/>
<br />
<br />
Copy picture into StegExample folder and rename it to pic.jpg. <br/>

<img src="https://imgur.com/xxT4Tmk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create a new text file by right-clicking in the folder and selecting New > Text Document and name it Secret1. Make sure it has a .txt file. <br/>
<img src="https://imgur.com/NmBrOwD.png" height="80%" width="80%" alt=""/>
<br />
<br />
Open the Secret1.txt file and type My Secrets into it, save and close it.. <br/>
<img src="https://imgur.com/aMpwOjv.png" height="80%" width="80%" alt=""/>    
<br />
<br />
Use WinRAR to compress the .txt file by clicking Add to Secret1.rar.. <br/>
<img src="https://imgur.com/EQNkTnt.png" height="80%" width="80%" alt="s"/>
<br />
<br />
Click on the desktop icon find your folder Steg example and double-click on it in the Explorer window. Next, click on the folder icon to highlight the current directory, type cmd, and hit enter to bring up the cmd prompt window. <br/>
<img src="https://imgur.com/yw7Ru4G.png" height="80%" width="80%" alt=""/>
<img src="https://imgur.com/2g3xvGt.png" height="80%" width="80%" alt=""/>

Now type dir in the cmd line and hit enter. This will give you what is contained in the StegExample folder. <br/>
<img src="https://imgur.com/zRbVnIK.png" height="80%" width="80%" alt=""/> 

Next, we will enter the following in the cmd prompt Copy/b pic.jpg+Secret1.rar stegpic.jpg (see image for cmd prompt example). This will embed the secret1.rar file within the original pic.jpg file.  <br/>
<img src="https://imgur.com/5I3YBEx.png" height="80%" width="80%" alt=""/>


If you click on the Explorer window folders you should see something like this minus my copy .jpg pic that I created as backup and moved it to the desktop.  <br/>
<img src="https://imgur.com/ksuIqAL.png" height="80%" width="80%" alt=""/>

To extract the hidden file in the new pic named stegpic.jpg we will need to rename the extension to stegpic.rar. In the cmd prompt type the following: copy stegpic.jpg stegpic.rar.  <br/>
<img src="https://imgur.com/rc163FQ.png" height="80%" width="80%" alt=""/>

Now if we go back to the file explorer window we will see the following.  <br/>
<img src="https://imgur.com/ktjmBcj.png" height="80%" width="80%" alt=""/>

Now we can extract the hidden message by using the explorer window in the picture by extracting files.  <br/>
<img src="https://imgur.com/gBhHJY0.png" height="80%" width="80%" alt=""/>


Now you will see a new folder on the Explorer window called Stegpic. Open that to find the message embedded in the picture.  <br/>
<img src="https://imgur.com/i0KMIji.png" height="80%" width="80%" alt=""/>

Ok, now we can check if this works another way. Create a new folder on your desktop and name it Picture from email.  <br/>
<img src="https://imgur.com/oEGcUR9.png" height="80%" width="80%" alt=""/>

Now open your email and send the original stegpic.jpg from the StegExample folder to another email that you own. Open the 2nd email that you sent to download the image and copy it to a new folder called Picture from email. Below is my example of this.  <br/>
<img src="https://imgur.com/ex0dI3B.png" height="80%" width="80%" alt=""/>


Now to extract the hidden message. Right-click on the picture and extract the message using WinRar. A new .txt will appear. If you open this you will see the hidden embedded message in the picture. <br/>
<img src="https://imgur.com/TlxYQet.png" height="80%" width="80%" alt=""/>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
