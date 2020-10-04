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
<div id="top"></div>        
<div id="guided_tour" style="font-family:verdana;">
	<h1>Java OceanAtlas Application</h1>
	<h2>Download and installation instructions</h2>
	<div id="guided_tour_content">

<p>
  Java OceanAtlas (JOA) is a computer application written in Java.  JOA and its
  support files must be installed on your computer.  JOA cannot be opened/run
  from removable media such as a CD or DVD, nor can it be opened/run over a
  network.
</p>

<p>
 Installing JOA is accomplished by mainly unzipping a zip file or disk image on macOS or launching the JOA installer on Windows. See the platform specific installation instructions. A JOA installation is composed of the JOA application and its support files in a single folder/directory.
</p>

<p>Once you have installed JOA, you should have a folder/directory on your
computer with these contents:</p>
<p>Mac</p>
<div class="image">
  <img alt="List of folders: bathymetry, coastlines, Example Data Files, Java OceanAtlas 5.0, JOA_Support, lexicon.txt, ndeditsettings.txt, temp"
       src="assets/images/general_install_1.jpg">
</div>
<p>Windows</p>
<div class="image">
  <img alt="List of folders: bathymetry, coastlines, Example Data Files, Java OceanAtlas 5.0, JOA_Support, lexicon.txt, ndeditsettings.txt, temp"
       src="assets/images/general_install_2.jpg"">
</div>

<p>
  Most of these are essential - the JOA application itself will not run without
  information it looks for in some of the other files - and so all must be
  co-located in the same folder/directory on your computer.
</p>

<h3 id="support_files">Support Files</h3>
<h4>Bathymetry Add-ins</h4>
<p>
  If you would like to add higher-resolution ETOPO files, download any or all
  of these files and unzip them into the JOA_Support folder/subdirectory on
  your computer.
</p>
<p>
  Java OceanAtlas contains ETOPO-60 and ETOPO-20 files. These are binary files
  extracted from ETOPO-5 with bathymetry and elevations at 5-minute spatial
  resolution.
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
