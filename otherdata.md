---
layout : datapage
title : Other Data
ocean: Other
---

<section id="hero">
  <div class="hero-container">
  <br><br><br><br>
      <h1>Explore {{page.ocean}} Ocean Data</h1>
      <h2>Navigate to your desired data below</h2>
      <center><img src="assets/images/othervertical.jpg" alt="" class="responsive"></center>
  </div>
</section><!-- #hero -->

<section id="call-to-action1">
<section id="call-to-action3">
    <div class="container wow fadeIn">
        <div class="col-lg-9 text-center text-lg-left"  style="flex:0 0 100%;max-width:100%">
          <h3 class="cta-title1" style="text-align:center">About {{page.ocean}} Best Section Data</h3>
          <br>
          <p class="cta-text1" style="text-align:center">2200 mostly pre-1990 vertical sections based on SIO Professor Joseph Reid's World Ocean data collection. Other pre-1990s Atlantic, Indian, and Pacific basin scale sections, including from the highly-regarded GEOSECS, TTO, and SAVE expeditions. A collection of Arctic Ocean and Nordic Sea data is also provided.</p><br>
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
              {% for item in site.data.otherdata.section %}
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

</div>
