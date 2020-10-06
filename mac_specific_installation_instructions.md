---
layout : joadoclayout
title : Mac Installation Instructions
css: joa
---

<div id="container" class="joa joa_download_windows  row-fluid" style="max-width:125vh;text-align:left;">
<div id="main_content" class="contained span8" style="min-width:122vh">
<div id="top"></div>
	<h1>Java OceanAtlas Application</h1>
	<h2>{{page.title}}</h2>

<ul>
<li>You do not have to install a separate Java environment for JOA 5.5 </li>
<li>The installation process depends on what operating system you are using. To check what version of macOS is installed on your computer, go to the apple menu in the top left corner of your screen and select <b>About This Mac.</b> JOA 5.5 has been tested on versions 12-15 of macOS.</li>
</ul>


<h2>Installation on macOS Catalina (10.15) </h2>
<ol>
<li>You must download JOA 5.5 from Safari. Open Safari and go to Preferences. In the General tab, turn on Open “safe” files after downloading. This is necessary for JOA to install correctly.</li>

<img alt="Mac-1" src="assets/images/mac1.jpg">

<li>Download the Zip file.</li>

<li>When the download is finished, there will be a folder called Java OceanAtlas in your downloads folder that contains these files:</li>

<img alt="Mac-2" src="assets/images/mac2.jpg">

<li>Move or copy the Java OceanAtlas folder to the desired location on your computer. We recommend putting it in Applications.</li>
</ol>

<h2>Installation on macOS Sierra (10.12), High Sierra (10.13), and Mojave (10.14)</h2>
<ol>
<li>Download the DMG file </li>

<li>Double click Java OceanAtlas.dmg to open it. You will see this window:</li>

<img alt="Mac-3" src="assets/images/mac3.jpg">

<li>Drag the folder called Java OceanAtlas to the provided link to your Applications folder, or to the desired location on your computer. Do not run JOA directly from the DMG.</li>

<li>You will see these files in the Java OceanAtlas folder. You can now eject the DMG from finder or unmount it using the Disk Utility application. The DMG can be kept as a backup or discarded entirely.</li>

<img alt="Mac-2" src="assets/images/mac2.jpg">
</ol>

<h2>Fixing Blurry Fonts in JOA</h2>
<p>If you are using Mojave or Catalina, you may notice certain text to be poorly rendered and difficult to read, such as colorbar labels: <br>
<img alt="Mac-4" src="assets/images/mac4.jpg">
<ol>
<li>Quit JOA. Open Terminal (Terminal can be found in your /Applications/Utilities/ folder). You will see some text in your Terminal window. The gray box is your cursor.</li>
<li>Copy and paste the following text into Terminal and press return: <br><br>
	<center><p style="font-family:Consolas">defaults write -g CGFontRenderingFontSmoothingDisabled -bool NO</p></center>
</li>
<img alt="Mac-5" src="assets/images/mac5.jpg">
<li>After you press return, a new line of text with your computer and account name will appear. There will be nothing to indicate that a change has taken effect. Quit terminal and restart JOA. If text still appears fuzzy, try logging out of your account and logging back on.</li>
</ol>
</p>

<h2>System Requirements:</h2>
<p>
JOA 5.5: macOS 10.12 or higher (may work under previous versions of macOS but has not been tested) <br>
JOA 5.3: Mac OS X 10.10 or higher<br>
JOA 5.2.1: Mac OS X 10.9 or lower<br>
4 GB of RAM (standard version) or 16 GB of RAM (pro version)
</p>
