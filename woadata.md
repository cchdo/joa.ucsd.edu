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
<div class="rightbox" style="width:100%; padding:0">
<div class="container h-100" style="width:75%">
<div class="row h-100 align-items-center justify-content-center">
<div class="col-12 col-md-10">
<div class="hero-search-form">
<div class="tab-content" id="nav-tabContent">
<div class="tab-pane fade show active" id="nav-places" role="tabpanel" aria-labelledby="nav-places-tab">
<h6>What data are you looking for?</h6>
<div class="row">
<form action="#" method="get" style='padding: 0px 17.5vw'>
  <select class="custom-select" id="verticalSectionDropdown" style='width: 13vw'>
    <option value="All" selected="selected">Vertical Section</option>
    {% for item in site.data.woadata.section%}
    <option value="{{item.title}}">{{item.title}}</option>
    {% endfor %}
  </select>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <select class="custom-select" id="yearDropdown" style='width: 13vw'>
    <option value="All">Subsection</option>
    {% for item in site.data.woadata.yeardropdown %}
    <option value="{{item.year}}">{{item.year}}</option>
    {% endfor %}
  </select>
  <select class="custom-select" id="fileDropdown" hidden>
  <option value="All">File</option>
  <option value=".csv">.csv</option>
  <option value=".jos">.jos</option>
  <option value=".txt">.txt</option>
  <option value=".joa">.joa</option>
  <option value=".zip">.zip</option>
  </select>
</form>
</div>
</div>
</div>
</div>
</div>
</div>
</div>
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
  <div class="limiter">
    <div class="container-table100" style='padding: 5vh 10vw'>
      <div class="wrap-table100" style='width: 80vw'>
        <div class="table100 ver3 m-b-110">
          <div class="table100-head">
            <table>
            <thead>
            <tr class="row100 head">
                <th class="cell100 column1">Vertical Section</th>
                <th class="cell100 column2">Subsection</th>
                <th class="cell100 column4">File</th>
            </tr>
          </thead>
        </table>
        </div>
        <div class="table100-body js-pscroll" style="max-height:1500px">
            <table class="table" id="datatable1">
            <tbody id="datatable">
            {% for item in site.data.woadata.section%}
            {% for entry in item.years%}
            {% for file in entry.files%}
              <tr>
                  <td class="cell100 column1">{{item.title}}</td>
                  <td class="cell100 column2">{{entry.year}}</td>
                  <td class="cell100 column4"><a href="{{file.path}}">{{file.name}}</a></td>
                </tr>
            {% endfor %}
            {% endfor %}
            {% endfor %}
            </tbody>
            </table>
</div>
</div>
</div>
</div>
</div>
</div>
</div>