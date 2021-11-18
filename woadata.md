---
layout : datapage
title : World Ocean Atlas Datapage
ocean: World Ocean Atlas
---

<section id="hero">
	<div class="hero-container">
		<br><br><br><br>
		<h1>Explore {{page.ocean}} Ocean Data</h1>
		<h2>Navigate to your desired data below</h2>
		<center><img src="assets/images/woamap.jpg" alt="" class="responsive"></center>
	</div>
</section>
<!-- #hero -->
<section id="call-to-action1">
	<section id="call-to-action3">
		<div class="container wow fadeIn">
			<div class="col-lg-9 text-center text-lg-left"  style="flex:0 0 100%;max-width:100%">
				<h3 class="cta-title1" style="text-align:center">About {{page.ocean}} Data</h3>
				<br>
				<p class="cta-text1" style="text-align:center">The NOAA World Ocean Atlas (WOA) quality-controlled mean temperature, salinity, dissolved oxygen, and nutrient data were originally released by layer by layer on standard level surfaces on a 1-degree positional grid for the World Ocean. We have WOA data from NOAA WOA releases from 1998, 2005, 2009, 2013, and 2018. We reassembled the data at each grid point into vertical profiles, with data at each WOAyy standard level for which there are reported values. We provide some of the WOAyy data as areal, gridded data at the original 1-degree grid spacing, and most at a sub-grid spacing which provides adequate basin-scale visualization with reduced computer resource requirements. Various collections of these grids and sub-grids are provided. We also provide vertical sections taken from WOAyy at 5-degree intervals of latitude and 10-degree intervals of longitude.</p>
			</div>
		</div>
	</section>
</section>
<!-- #call-to-action -->
<div id="collapseDVR3" class="panel-collapse collapse in" style="background-color: black">
<center>
  <div class="tree ">
    <ul>
      <span style="color:white;font-size:large"><b><u>{{page.ocean}} Data</u></b></span>
      <ul>
        <li>	<span style="background:#5cb85c;color:white">Download all {{page.ocean}} Data</span></li>
        {% for item in site.data.woadata.section %}
        <li>
          <span style="color:white"><i class="fa fa-plus-square" style="color:white"></i>{{item.title}}</span>
          <ul>
            <li>	<span style="background:#5cb85c;color:white">Download all {{item.title}} Data</span></li>
            {% for entry in item.years%}
            <li>
              <span style="color:white"><i class="fa fa-plus-square" style="color:white"></i>{{entry.year}}</span>
              <ul>
                <li> <span style="color:white">File</span> </li>
                <li> <span style="color:white">File</span> </li>
                <li> <span style="color:white">File</span> </li>
                <li> <span style="color:white">File</span> </li>
              </ul>
            </li>
            {% endfor %}
          </ul>
        </li>
        {% endfor %}
      </ul>
    </ul>
  </div>
</center>
