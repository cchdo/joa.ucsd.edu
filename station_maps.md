---
layout : joalayout
title : Station Maps
css: joa
---

<center>
<div id="container" class="tour page  row-fluid" style="max-width:125vh;text-align:left;">
<div id="main_content" class="contained span8">
<div id="top"></div>
<div id="guided_tour" style="font-family:verdana;">
	<h1>Guided Tour of Java OceanAtlas </h1>
	<h2>{{page.title}}</h2>
	<div id="guided_tour_content">

<p>Plots are the heart of the application. One of the first questions you might have would be &lsquo;where are these data located?&rsquo; Java OceanAtlas includes station maps.<br><br>
	Select &lsquo;Map...&rsquo; from the Plots menu. The will bring up the Configure Map Plot dialog box.
</p>

<p style="padding-left:35px;">
	We have configured the dialog boxes for each JOA plot type so that a basic plot can be made with a minimum of user input.
	<br><br>
	For a JOA map plot, no further user inputs are required: the &lsquo;Plot&rsquo; button is activated, meaning a basic map plot will be drawn by clicking on the &lsquo;Plot&rsquo; button.
</p>

<p>
	In this Guided Tour we show some basic plot customization features:<br><br>
	Select the &lsquo;Miller&rsquo; projection from the scrollable list of projections.
	<br><br>
	Select the &lsquo;Central Atlantic&rsquo; preset region. In the 'Latitude spacing (deg)&rsquo; and Longitude spacing (deg)&rsquo; boxes select the pre-set text and type in '10&rsquo; and '20&rsquo;, respectively. Java OceanAtlas maps include default bathymetry based on the ETOPO60 one-degree coarse grid: click the 'bathymetry&rsquo; tab to see this (on a new copy of JOA it is set up this way by default). The dialog box should look like the examples in Figure 2.
 <br><br>
<img alt="Gt_fig-02a" class="gt_image" src="assets/images/fig2.png">
</p>

<p>Then click 'Plot'. You will see a map with the stations, shaded land masses, gray bathymetry, and a latitude/longitude grid, as shown in Figure 3.<br><br>
    <img alt="Gt_fig-03" class="gt_image" src="assets/images/fig3.png"></p>

<p>Map plots show individual dots for each station, with a different station color for each section subset. (JOA determines this coloring for reasons mostly ignored here, for example when there is more than one section opened.) In Figure 3 the apparent 'cruise line' is actually a series of 80 individual station dots. The map window is scrollable and resizable. (You may need to click on the 'Reset' button in the map plot window to force a redraw.) Selecting a subset of the plot by click-dragging the cursor will produce a subset of the map plot covering only the selected area. [Sometimes, due to a Java quirk, the new map subset plot is initially hidden under the original map plot window.]</p>
	</div>
	</div>
			</div>     
			<div id="right" class="span4">        
	<h1>Guided Tour of Java OceanAtlas</h1>
	<ul>
	<li><a href="basic_features.html">Basic Features</a></li>
	<li><a href="starting_joa.html">Starting JOA</a></li>
	<li class="active"><a href="station_maps.html">Station Maps</a></li>
	<li><a href="profile_plots.html">Profile Plots</a></li>
	<li><a href="changing_color_bar.html">Changing Color/Contour Bar</a></li>
	<li><a href="calculate_parameters.html">Calculate Parameters</a></li>
	<li><a href="property_plots.html">Property-Property Plots</a></li>
	<li><a href="browsing.html">Browsing</a></li>
	<li><a href="modifying_plots.html">Modifying Plots</a></li>
	<li><a href="extracting_selections.html">Extracting Selections</a></li>
	<li><a href="contour_plots.html">Contour Plots</a></li>
	<li><a href="other_features.html">Other Features</a></li>
	<li><a href="more_about_maps.html">More About Maps</a></li>
	<li><a href="how_to_filter_your_data.html">How to Filter Your Data</a></li>
	<li><a href="final_remarks.html">Final Remarks</a></li>
	<li><a href="joa_data_files.html">Java OceanAtlas Data Files</a></li>
	</ul>

	<p><a class="cta-btn align-middle" href="joa.html">Explore</a></p>
	        </div>       
	      </div>
	</center>
