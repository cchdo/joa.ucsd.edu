---
layout : datapage
title : Other Data
ocean: Other
---

<section id="hero">
  <div class="hero-container">
  <br><br>
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
          <p class="cta-text1" style="text-align:center">Global-scale vertical sections assembled by J. Swift from the Best Vertical Sections, intended to illuminate the largest-scale spatial structure of seawater characteristics. The data have been vetted and groomed for improved readability and consistency, and assembled in sensible geographic order.</p><br>
          <p class="cta-text1" style="text-align:center">A collection of carefully-matched section segments from all of the oceans - crossings of the same path in one basin or region from different years. These are included to facilitate accurate comparisons of seawater characteristics from different years. Data file names are designed to identify spacially-matched sets.</p>
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
