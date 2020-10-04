---
css: joa
---
<!DOCTYPE html>
<html lang="{{ site.lang | default: "en-US" }}">

{% include joa_head.html %}
<style>
body {
  width: 100%;
  height: 100vh;
  background-size: cover;
  position: relative;
  background-color: lightblue;
	}
.cta-btn {
  font-family: "Poppins", sans-serif;
  text-transform: uppercase;
  font-weight: 500;
  font-size: 16px;
  letter-spacing: 1px;
  display: inline-block;
  padding: 8px 30px;
  border-radius: 50px;
  transition: 0.5s;
  border: 2px solid #000000;
  color: #000000;
}

.cta-btn:hover {
  background: #2dc997;
  border: 2px solid #2dc997;
}


</style>
  <body>

{% include joaheader.html %}

<br><br><br><br><br>
<center>
<div id="container" class="tour page  row-fluid" style="max-width:125vh;text-align:left;">
<div id="main_content" class="contained span8">
<div id="top">Java OceanAtlas Application</div>        
<div id="guided_tour" style="font-family:verdana;">
	<h3>Windows Installation Instructions</h3>
	<div id="guided_tour_content">

<h2>Installation</h2>
<p>After downloading, just double-click installer icon to begin installation process:<br>
<img alt="Windows-1" src="assets/images/windows1.jpg"></p>

<p>You will be presented with a series of dialogs to guide you through the installation process:<br>
<img alt="Windows-2" src="assets/images/windows2.jpg"></p>

<p>Select an installation folder if different than the default:<br>
<img alt="Windows-3" src="assets/images/windows3.jpg></p>

<p>Click Install to install JOA onto your PC:  <br>
<img alt="Windows-4" src="assets/images/windows4.jpg"></p>

<p>Click Finish at the end of the installation process:<br>
<img alt="Windows-5" src="assets/images/windows5.jpg></p>

<h3>Windows System Requirements</h3>
<p>
JOA 5.5: Microsoft Windows 10 (may work under earlier version of Windows but has not been tested)<br>
JOA 5.3: Microsoft Windows 8 or 8.1 (not tested under Windows 10)<br>
JOA 5.2.1: Microsoft Windows XP or Windows 7<br>
4 GB of RAM (JOA 5.5 standard version, earlier versions of JOA) or 16 GB of RAM (JOA 5.5 pro version)
</p>


</div>
</div>
    </div>      
  </div>
</center>
<br><br>

{% include footer.html %}

</body>
</html>
