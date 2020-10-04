---
layout : joadoclayout
title : Managing Java OceanAtlas Features
css: joa
---
<div id="container" class="joa features  row-fluid" style="max-width:125vh;text-align:left;">
<div id="main_content" class="contained span8" style="min-width:122vh">
<div id="top"></div>
	<h1>Java OceanAtlas Application</h1>
	<h2>{{page.title}}</h2>

<p>The JOA application was written originally to be the application centerpiece of an electronic
atlas of ocean profile data. The application has evolved and grown as users suggested new
features and the authors conceived many of their own. Some specialty users needed features
directed primarily at their interests. Also, while most JOA features are robust, some are still
in development, or simply quirky. And the authors agree that a version of JOA with too many
features up front would make JOA much less easy to use for first-time users.</p>

<p>Our solution has been to create a Feature Manager, accessible as one of the choices in the JOA
Preferences dialog box, accessed from the &quot;Java OceanAtlas&quot; menu on Mac OS X and under the
Edit menu on Windows and Linux. Through the Feature Manager, various JOA features can be
turned on and off.</p>

<p>The default JOA enabled-feature set in the downloaded application is a balance between
simplicity and power, chosen by Swift to match the needs of graduate student users of JOA,
for example, students using the JOA DPO Examples. Educators who wish a simpler JOA for
their students may want to turn off some of the default enabled features. Meanwhile, power
users, or those curious to see what more lies within JOA, may want to experiment with enabling
additional JOA features. Typically each feature adds one or more choices to the JOA menus.</p>

<p>Most JOA features are discussed in the JOA User Guide (available to the right).</p>

<p>We include, below, a list of the JOA features which can be turned on and off via the JOA Feature
Manager. Note that &quot;Objective Analysis&quot; is still under development, &quot;Gradient Contour Plots&quot;
permit plotting sections of geostrophic velocity, and &quot;Station Calculation XY Plots&quot; can be
interesting and useful.</p>

<p>As we add new features to JOA, and complete implementation of some existing features, the
choices in the JOA Feature Manager will change.</p>

<h2>List of Managed Features</h2>
<div id="feature_list">
  <h3 class="feature_type">Filters</h3>
  <ul>
    <li>Allow Observation Filtering</li>
    <li>Allow Station Filtering</li>
  </ul>

  <h3 class="feature_type">File Options</h3>
  <ul>
    <li>Export EPIC Pointer file</li>
    <li>Allow File Merge</li>
    <li>Allow Exporting Station Calculations</li>
    <li>Access Dapper Servers</li>
    <li>Export WOCE Exchange Files</li>
    <li>Export netCDF Section</li>
    <li>Export Spreadsheet Files</li>
  </ul>

  <h3 class="feature_type">Calculations</h3>
  <ul>
    <li>Allow Station Calculations</li>
    <li>Allow Custom Station Calculations</li>
    <li>Allow Parameter Calculations</li>
    <li>Allow Section Calculations</li>
    <li>Allow Modeling TS relationships</li>
    <li>Allow Custom Calculations</li>
    <li>Allow Value Recoding</li>
    <li>Allow Parameter Transformations</li>
  </ul>

  <h3 class="feature_type">NdEdit Options</h3>
  <ul>
    <li>Allow NdEdit Browsing</li>
    <li>Allow Overlay Contours on Map Plots</li>
    <li>Overlay Contours Based on a Calculated Station Parameter</li>
    <li>Overlay Contours Based on an Isosurface</li>
  </ul>

  <h3 class="feature_type">Contour Plots</h3>
  <ul>
    <li>Objective Analysis in Interpolation</li>
    <li>Overlay Contours</li>
  </ul>

  <h3 class="feature_type">Plots</h3>
  <ul>
    <li>Allow Station Calculation Plots</li>
    <li>Allow Gradient Contour Plots</li>
    <li>Allow Profile Plots</li>
    <li>Allow Line Plots</li>
    <li>Allow Map Plots</li>
    <li>Allow Contour Plots</li>
    <li>Allow Station Calculation XY Plots</li>
    <li>Allow Property-Property Plots</li>
  </ul>

  <h3 class="feature_type">Station Calculations</h3>
  <ul>
    <li>Allow Neutral Surface Calculations</li>
    <li>Allow Windspeed and Direction Calculations</li>
    <li>Allow Station Statistics Calculations</li>
    <li>Allow Interpolations Calculations</li>
    <li>Allow Integration Calculations</li>
    <li>Allow Mixed-layer Depth Calculations</li>
    <li>Allow Extrema Calculations</li>
  </ul>

  <h3 class="feature_type">Map Station Colors</h3>
  <ul>
    <li>Station Coloring Based on Station Metadata</li>
    <li>Station Coloring Based on an Isosurface</li>
    <li>Station Coloring Based on a Calculated Station Parameter</li>
  </ul>

  <h3 class="feature_type">Resource Editors</h3>
  <ul>
    <li>Allow Editing/Creating Interpolation Surfaces</li>
    <li>Allow Editing/Creating Color Bars</li>
    <li>Allow Editing/Creating Color Palettes</li>
  </ul>

  <h3 class="feature_type">Preferences</h3>
  <ul>
    <li>Show General Preferences</li>
    <li>Show CTD Decimation Preferences</li>
    <li>Import World Ocean Data Select CSV Files</li>
    <li>Show Enhancement Preferences</li>
    <li>Show Parameter Substitutions Preferences</li>
    <li>Show Import Preferences</li>
    <li>Allow Users to Manage Features</li>
    <li>Show Font Preferences</li>
  </ul>

  <h3 class="feature_type">Section Calculations</h3>
  <ul>
    <li>Allow Section Difference Calculations</li>
    <li>Allow Mean Cast Calculations</li>
  </ul>

  <h3 class="feature_type">Section Editors</h3>
  <ul>
    <li>Show Section Manager</li>
    <li>Allow Editing Parameter properties</li>
    <li>Use NQuery Database Features</li>
    <li>Allow Station Data Editing</li>
    <li>Allow Editing File Properties</li>
  </ul>
</div>
