---
layout : datapage
title : Indian Datapage
ocean: Indian
---



<section id="call-to-action1">
<section id="call-to-action3">
    <div class="container wow fadeIn">
        <div class="col-lg-9 text-center text-lg-left"  style="flex:0 0 100%;max-width:100%">
          <h3 class="cta-title1" style="text-align:center">About {{page.ocean}} Ocean Data</h3>
          <br>
          <p class="cta-text1" style="text-align:center">We have prepared ca. 2200 vertical sections from the original NODC data files contributing to SIO Professor Joseph Reid's ‘pre-WOCE’ (pre-1990s) World Ocean data collection. From the many thousands of cruises in NODC Archives, and some newer cruises originally from colleagues, over more than two decades Joe sifted for the best available data from each region of the World Ocean (except for the Arctic). His intended purpose was to make maps of water properties, and so he cut off stations from a cruise where a better (better for his purposes) cruise overlapped it. He made corrections to many of the data for known offsets (mostly standard seawater batch offsets). Here we went into the NODC files and retrieved the entire cruise data set for each cruise Joe used, assembled the stations into sensible vertical sections, applied the same corrections Joe used, and then we culled many bad data values. The resulting 2200 sections represent the basic data knowledge of the deep ocean basins prior to the 1990s. The data sets all include temperature and salinity, nearly all have dissolved oxygen data, and most have nutrient (NO3, PO4, and/or SiO3) data.</p>
        </div>
      </div>
</section>
</section><!-- #call-to-action -->

<div id="collapseDVR3" class="panel-collapse collapse in" style="background-color: black">
<div class="tree ">
   <ul>
       <span style="color:white;font-size:large"><b><u>{{page.ocean}} Ocean</u></b></span>
           <ul>
              <li>	<span style="background:#5cb85c;color:white">Download all {{page.ocean}} Data</span></li>
              {% for item in site.data.indiandata.section %}
               <li>
               	<span style="color:white"><i class="fa fa-plus-square" style="color:white"></i>{{item.title}}</span>
                 <ul>
                   <li>	<span style="background:#5cb85c;color:white">Download all {{item.title}} Data</span></li>
                   {% for entry in item.years%}
                     <li>	<span style="color:white"><i class="fa fa-plus-square" style="color:white"></i>{{entry.year}}</span>
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

<div class="rightbox">
<div class="container h-100" style="width:80%">
<div class="row h-100 align-items-center justify-content-center">
<div class="col-12 col-md-10">
<div class="hero-search-form">
<div class="tab-content" id="nav-tabContent">
<div class="tab-pane fade show active" id="nav-places" role="tabpanel" aria-labelledby="nav-places-tab">
<h6>What data are you looking for?</h6>
<div class="row">
<form action="#" method="get">
<center>
  <select class="custom-select" id="verticalSectionDropdown">
    <option value="All" selected="selected">Vertical Section</option>
    {% for item in site.data.indiandata.section%}
    <option value="{{item.title}}">{{item.title}}</option>
    {% endfor %}
  </select>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <select class="custom-select" id="yearDropdown">
    <option value="All">Year</option>
    {% for item in site.data.indiandata.yeardropdown %}
    <option value="{{item.year}}">{{item.year}}</option>
    {% endfor %}
  </select>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <select class="custom-select" id="fileDropdown">
    <option value="All">File</option>
    <option value="Basin">.csv</option>
    <option value="Sub Basin">.jos</option>
    <option value="Option_3">.txt</option>
    <option value="Option_4">.joa</option>
    <option value="Option_5">.zip</option>
  </select>
</center>
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
    <div class="container-table100">
      <div class="wrap-table100">
        <div class="table100 ver3 m-b-110">
          <div class="table100-head">
            <table>
            <thead>
            <tr class="row100 head">
                <th class="cell100 column1">Vertical Section</th>
                <th class="cell100 column2">Year</th>
                <th class="cell100 column4">File</th>
            </tr>
          </thead>
        </table>
        </div>
        <div class="table100-body js-pscroll" style="max-height:1500px">
        <table class="table" id="datatable1">
        <tbody id="datatable">
        {% for item in site.data.indiandata.section%}
        {% for entry in item.years%}
          <tr>
              <td class="cell100 column1">{{item.title}}</td>
              <td class="cell100 column2">{{entry.year}}</td>
              <td class="cell100 column4">{{entry.file}}</td>
            </tr>
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
