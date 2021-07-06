---
layout : default
css: main
title : Welcome to the Java OceanAtlas Suite
description : Explore cleaned, vetted World Ocean Bottle and CTD Profile Data
section_1:
  title: About the Java OceanAtlas Suite
section_2_title : About Java OceanAtlas
section_3_title :   About the Data on the Website
ocean_counter : 5
verticalsection_counter : 232
year_counter : 39
cruise_counter: 1463

---
<link rel="stylesheet" href="/assets/css/main.css">
<section id="hero">
  <div class="hero-container">
    <br><br><br><br><br>
      <h1>{{page.title}}</h1>
      <h2>{{page.description}}</h2>
          <div style="display: inline-block;">
              <br><br>
        <a href="Data_homepage" class="btn-get-started">Dive in &rarr;</a>
      </div>
      <br><br><br><br><br>
      <div style="display: inline-block;">
        <a href="#call-to-action" class="btn-get-started1">Archives</a>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
        <a href="#facts" class="btn-get-started1">Statistics</a>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
        <a href="#contact" class="btn-get-started1">Contact</a>
      </div>
</div>
</section>

<main id="main">

<!--==========================
  About Us Section
============================-->
<section id="about">
  <div class="container">
    <div class="row about-container">

      <div class="col-lg-15 content order-lg-1 order-2">
        <h2 class="title">{{page.section_1.title}}</h2>
        <p>
          The Java OceanSuite includes
            <ul>
                <li>Downloads, documentation and support files for the Java OceanAtlas (JOA) application for Windows and MacOS,</li>
                <li>an extensive collection of groomed World Ocean vertical profile water sample and CTD data in ASCII WHP-Exchange and JOA binary formats,</li>
                <li>a virtual research cruise to the far southeast Indian Ocean aboard SIO's R/V Roger Revelle, and</li>
                <li>suggestions and support for data analysis and exploration projects.</li>
            </ul>
        </p>
      </div>
    </div>

  </div>
</section><!-- #about -->

    <section id="about" style="background:black">
  <div class="container">
    <div class="row about-container">

      <div class="col-lg-15 content order-lg-1 order-2" style="background:black;color:white;text-align:justify">
        <h2 class="title" style="color:white;text-align:right">{{page.section_2_title}}</h2>
        <p>
          Java OceanAtlas (JOA) is a Java application for Windows and MacOS which provides an ad hoc (rather than pre-set) graphic exploration environment optimized to examine and plot oceanographic profile data. JOA works with any pressure- or depth-indexed data, for example 'WHP-Exchange' data, such as from the CLIVAR and Carbon Hydrographic Data Office (CCHDO;<a href="https://cchdo.ucsd.edu/">https://cchdo.ucsd.edu</a>).
          <br><br>
          Java OceanAtlas plots include property-property plots, maps, offset profiles (waterfall), contour plots, and plots of calculated values, using color-by-property-value as a plotted variable to aid interpretation. There is also a comprehensive data display window and extensive support for data editing and quality control functions. All Java OceanAtlas plots and the data window are linked and may be ‘browsed’ jointly by sample and/or station. Plots can be re-scaled, re-sized, or have their colored variable changed. Selected areas of profile, property-property, contour plots, maps, and station value plots can be extracted into new plots. Standard levels, scales, contours, and colors can be changed via user interfaces similar to those used in commercial applications. Java OceanAtlas provides data filtering and exporting. Many different types of calculations can be performed.
        </p>
      </div>
    </div>

  </div>
</section><!-- #about -->




<section id="about">
  <div class="container">
    <div class="row about-container">
      <div class="col-lg-15 content order-lg-1 order-2">
        <h2 class="title">{{page.section_3_title}}</h2>
        <p>
          The data provided here were prepared to provide students and researchers a collection of the best available 'blue water' ocean vertical profiles. Most data are in both ASCII WHP-Exchange and Java OceanAtlas binary formats. We have added value to many of these data by organizing sections, by combining and deleting stations, and by correcting some errors. Note that we continually update the data, replacing data files with preferred versions or adding cruises, old and new, to the collection.
          <br><br>
         The collection 'Best Vertical Section Data' contains some of the finest-quality vertical section bottle and CTD data yet obtained from the World Ocean, from WOCE, CLIVAR, GO-SHIP and other programs of similar focus and quality. Includes a compilation of matched section segments - crossings of the same path in one basin or region from different years.
          <br><br>
          The collection 'World Ocean Atlas Data' contains vertical profile data extracted for mapping and vertical sections from various iterations of the NOAA/NCEI/NODC World Ocean Atlas data, originally on standard level surfaces on a 1-degree positional grid for the World Ocean.
          <br><br>
          The collection 'Other Data Files' contains ≈2200 vertical sections from the original NODC data files contributing to SIO Professor Joseph Reid's pre-WOCE (pre-1990s) World Ocean data collection, an assortment of other pre-WOCE vertical section data of interest, a collection of Arctic Ocean and Nordic Seas data, and a special collection of data files meant to be used, chapter by chapter, with the DPO JOA Examples which accompany the Talley et al. textbook,<b>Descriptive Physical Oceanography.</b>
          <br><br>
           &nbsp;&nbsp;&nbsp;&nbsp;<i>J.Swift</i>
        </p>
      </div>
    </div>

  </div>
</section><!-- #about -->

<!--==========================
  Facts Section
============================-->
   <section id="facts">
  <div class="container wow fadeIn">
    <div class="section-header">
      <h3 class="section-title"><font color="white">Statistics</font></h3>
      <p class="section-description">World Ocean Data cumulated into a nutshell</p>
    </div>
    <div class="row counters">

      <div class="col-lg-3 col-6 text-center">
        <span data-toggle="counter-up">{{page.ocean_counter}}</span>
        <p><font color="white">Oceans</font></p>
      </div>

      <div class="col-lg-3 col-6 text-center">
        <span data-toggle="counter-up">{{page.verticalsection_counter}}</span>
        <p><font color="white">Vertical Sections</font></p>
      </div>

      <div class="col-lg-3 col-6 text-center">
        <span data-toggle="counter-up">{{page.year_counter}}</span>
        <p><font color="white">Years of Cumulative Data</font></p>
      </div>

      <div class="col-lg-3 col-6 text-center">
        <span data-toggle="counter-up">{{page.cruise_counter}}</span>
        <p><font color="white">Cruises</font></p>
      </div>

    </div>

  </div>
</section><!-- #facts -->

<!--==========================
  Services Section
============================-->
<section id="services">
  <div class="container wow fadeIn">
    <div class="section-header">
      <h3 class="section-title">Datasets</h3>
      <p class="section-description">The data sets provided at this website were put together in order to provide Java OceanAtlas users a collection of the best available 'blue water' ocean vertical profile data for education and research use</p>
    </div>
    <div class="row">
      <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.2s">
        <div class="box">
          <h4 class="title"><a href="Data_homepage#call-to-action"><u>Vertical Section Data</u></a></h4>
          <p class="description">Cleaned versions of some of the finest World Ocean vertical section CTD and bottle data yet obtained, for education and research use. WHP-Basin Scale Sections.</p>
        </div>
      </div>
      <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.4s">
        <div class="box">
          <h4 class="title"><a href="Data_homepage#call-to-action1"><u>World Ocean Atlas Data</u></a></h4>
          <p class="description">Temperature, salinity, oxygen, and nutrient data extracted from the Levitus et al. WOA averaged property fields; on sub-grids and on vertical sections.</p>
        </div>
      </div>
      <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.2s">
        <div class="box">
          <h4 class="title"><a href="Data_homepage#call-to-action2"><u>Other Data Files</u></a></h4>
          <p class="description">Pre-1990s sections for examining basin-scale ocean water properties, a collection of Arctic and Nordic Sea data, and a few custom-made data files.</p>
        </div>
      </div>
    </div>

  </div>
</section><!-- #services -->

<!--==========================
Call To Action Section
============================-->
<section id="call-to-action">
  <div class="container wow fadeIn">
    <div class="row">
      <div class="col-lg-9 text-center text-lg-left">
        <h3 class="cta-title">Outreach</h3>
        <p class="cta-text">A virtual research cruise to the far southeast Indian Ocean aboard SIO's R/V Roger Revelle: tour the ship, watch videos of activities at sea and interviews with students, crew, techs, officers, and scientists, read the weekly reports, read the NSF proposal that funded the cruise, examine some aspects of the data, etc.</p>
      </div>
      <div class="col-lg-3 cta-btn-container text-center">
        <a class="cta-btn align-middle" href="{{'/outreach/virtualcruise/' | relative_url}}">Explore</a>
      </div>
    </div>

  </div>
</section><!-- #call-to-action -->

<section id="contact">
  <div class="container wow fadeInUp">
    <div class="section-header">
      <h3 class="section-title">Contact Us</h3>
      <p class="section-description"></p>
    </div>
  </div>
  <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3351.1581131516714!2d-117.25382838422442!3d32.867535780944706!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x80dc0754e9b63c47%3A0xf54d1be123616ebe!2sDeep%20Sea%20Drilling%20West%20Building!5e0!3m2!1sen!2sus!4v1589926372098!5m2!1sen!2sus" width="100%" height="380" frameborder="0" style="border:0" allowfullscreen></iframe>

  <div class="container wow fadeInUp mt-5">
    <div class="row justify-content-center">

      <div class="col-lg-3 col-md-4">

        <div class="info">
          <div>
            <i class="fa fa-map-marker"></i>
            <p>Room #50<br>Deep-Sea Drilling West<br>2215 Downwind Way<br>La Jolla, CA 92037</p>
          </div>

          <div>
            <i class="fa fa-envelope"></i>
            <p>jswift @ucsd.edu</p>
          </div>
        </div>

      </div>

    </div>

  </div>
</section><!-- #contact -->

</main>

<footer id="footer">
  <div class="footer-top">
    <div class="container">

    </div>
  </div>

  <div class="container">
    <div class="credits">
      <!--
        All the links in the footer should remain intact.
        You can delete the links only if you purchased the pro version.
        Licensing information: https://bootstrapmade.com/license/
        Purchase the pro version with working PHP/AJAX contact form: https://bootstrapmade.com/buy/?theme=Regna
      -->
      <a href="https://www.nsf.gov/"><img src="assets/images/logo_nsf.svg" alt="NSF logo" height="60" width="60"></a>
      <a href="https://www.noaa.gov/"><img src="assets/images/logo_noaa_new.svg" alt="NOAA logo" height="60" width="280"></a>
      <a href="https://scripps.ucsd.edu/"><img src="assets/images/logo_sio_color.svg" alt="SIO logo" height="60" width="60"></a>
      <a href="http://www.clivar.org/"><img src="assets/images/logo_clivar.svg" alt="CLIVAR logo" height="60" width="95"></a>
      <a href="https://www.go-ship.org/"><img src="assets/images/logo_goship.svg" alt="GO-SHIP logo" height="60" width="60"></a><br />
      <small>Any opinions, findings, and conclusions or recommendations expressed in this material are those of Dr James Swift and do not necessarily reflect the views of the supporting agencies.</small><br>
    </div>
  </div>
</footer><!-- #footer -->

<a href="#" class="back-to-top"><i class="fa fa-chevron-up"></i></a>
