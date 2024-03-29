---
layout : joalayout
title : Java OceanAtlas Data Files
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
					<p>Java OceanAtlas reads oceanographic data in several common or useful formats. Each of these is indicated to Java OceanAtlas when it tries to open a data file by virtue of its file extension, i.e. a mandatory suffix at the end of a data file name. The requirement for file extensions is necessary because Java OceanAtlas must work on many different platforms, and with several different operating systems underpinning its Java code. The list of presently-accepted data format file extensions, each with a description of that file type follows:</p>
					<table class="gt_data_table">
						<tr>
							<th>File extension (suffix)</th>
							<th>Description of the file format represented by the extension</th>
						</tr>
						<tr>
							<td>.joa</td>
							<td><b>Java OceanAtlas binary (read, write)</b>
								<br /> Good for storing custom sections as well as files that have been imported from other formats. Java OceanAtlas binary files will usually open significantly faster than importing files in plain text. Java OceanAtlas binaries store parameter units as well as bottle and observation quality codes.</td>
						</tr>
						<tr>
							<td>.jos</td>
							<td><b>Spreadsheet (TSV) (read, write)</b>
								<br /> A tab-separated (TSV) format that is compatable with most spreadsheet applications.</td>
						</tr>
						<tr>
							<td>.poa</td>
							<td><b>Power OceanAtlas binary (read, write)</b>
								<br /> These are files that were originally produced for Mac Power OceanAtlas. This format gives you access to large historical datasets created originally for OceanAtlas. These files do not store units or quality code information.</td>
						</tr>
						<tr>
							<td>_hy1.csv</td>
							<td><b>WOCE Bottle section in WHP-Exchange format (read)</b>
								<br /> This is a comma separated value fle (CSV) produced by the WOCE Hydrographic Program. Files in this format include multiple stations and usually correspond to a complete section or cruise. Java OceanAtlas provides 'post processing' capabilities to filter observations by quality code information as well as perform units conversion.</td>
						</tr>
						<tr>
							<td>_ct1.csv</td>
							<td><b>WOCE CTD profile in WHP-Exchange format (read)</b>
								<br /> This is a comma separated value file (CSV) produced by the WOCE Hydrographic Program. Files in this format include a single CTD cast. Java OceanAtlas preserves all units and quality codes. Java OceanAtlas provides significant 'post processing' to filter observations by quality information as well as units conversion. CTD files can be decimated to user-selected intervals or Java OceanAtlas standard levels.</td>
						</tr>
						<tr>
							<td>_ct1.zip</td>
							<td><b>WOCE CTD section in WHP-Exchange format (read)</b>
								<br /> A zip file that contains multiple individual CTD profiles.</td>
						</tr>
						<tr>
							<td>.nc</td>
							<td><b>netCDF Profile (read, write)</b>
								<br /> Individual CTD or bottle profiles that adhere to PMEL's EPIC standard. Future versions of Java O NODC
								<br /> <b>SD2 (read)</b>
								<br /> Text files that adhere to NODC's SD2 exchange format.</td>
						</tr>
					</table>
					<p>Note that Java OceanAtlas writes ('exports') data in four different formats (JOA Binary, POA Binary, JOA Spreadsheet, and netCDF Section). You can use Java OceanAtlas to read data in one of the other formats and translate into one of the four. Calculated parameters such as potential temperature and density can be added by Java OceanAtlas between reading and exporting the data, or data subsets or new sections can be made.</p>
					<p>You may be interested in having Java OceanAtlas read your own data. Spreadsheet format data are the easiest for most users to generate if they are not already familiar with writing data in one of the other supported formats. Fortunately, Java OceanAtlas spreadsheet format is not too demanding. Java OceanAtlas 'understands' many data headers, and reads data in column (spreadsheet) format. For example, an Excel file saved as comma- or tab- delimited text, set up to meet minimal Java OceanAtlas requirements, will read straight into JOA.</p>
					<p><u>Java OceanAtlas requires of each data set at least a <b>section name</b>, a <b>station number</b>, a <b>latitude</b>, a <b>longitude</b>, and <b>data at one level (one pressure)</b>.</u> Columns must be labeled. Java OceanAtlas will try to recognize heading names from its internal lexicon. The words shown below are recognized.</p>
					<p> <b>SECTION</b> names are short alphanumerics.
						<br>
						<br> <b>STATION</b> numbers are typically 1-4 digit numbers but can be alphanumerics.
						<br>
						<br> <b>LATITUDE</b>s are expressed in decimal degrees, positive in northern hemisphere and negative in the southern hemisphere.
						<br>
						<br> <b>LONGITUDE</b>s are expressed in decimal degrees, positive in eastern hemisphere and negative in the western hemisphere.</p>
					<p> Oceanographers use a left-handed coordinate system, meaning that while the X-axis and Y-axis point positive in the usual sense, the Z-axis is positive downward. Java OceanAtlas data are indexed by PRESsure, which is the parameter used most often for vertical orientation in physical oceanography. Because the pressure at 10 meters depth in the ocean is quite close to one bar, or one atmosphere, one decibar is nearly the same vertical extent as one meter. Decibars are the pressure unit used throughout oceanography and in Java OceanAtlas.</p>
					<p>
						<ul>
							<li>To make a simple data spreadsheet set, look up the latitude and longitude of your city, convert to decimal degrees, and substitute the name and position for 'YOURCITY', '35.00', and '-120.00' in the example:
								<br>SECTION&lt;tab&gt;STATION&lt;tab&gt;LATITUDE&lt;tab&gt;LONGITUDE&lt;tab&gt;PRES&lt;cr&gt; TEST&lt;tab&gt;YOURCITY&lt;tab&gt;35.00&lt;tab&gt;-120.00&lt;tab&gt;1.0&lt;cr&gt;
								<br />
								<br /> The use of '&lt;tab&gt;' in the above denotes a tab character, and '&lt;cr&gt;' denotes a carriage return.</li>
						</ul>
					</p>
					<p>This two-line file, if saved as plain text and with a file name given a '.jos' suffix, can be opened by Java OceanAtlas. If you then do a map plot, you will find a station dot at the position you provided.</p>
					<p>It is only a small extension from this minimum example to see the makings of a small Java OceanAtlas spreadsheet data file holding oceanographic profile data, shown below as a table:</p>
					<table class="gt_data_table">
						<tr><th>STATION</th><th>LATITUDE</th><th>LONGITUDE</th><th>PRES</th><th>TEMP</th><th>SALT</th><th>O2</th></tr>
						<tr><td>312</td><td>64.002</td><td>-27.833</td><td>16	</td><td>8.0754</td><td>35.0699	</td><td>7.25</td></tr>
						<tr><td>312</td><td>64.002</td><td>-27.833</td><td>49	</td><td>7.6206</td><td>35.0744	</td><td>6.89</td></tr>
						<tr><td>312</td><td>64.002</td><td>-27.833</td><td>99	</td><td>7.4723</td><td>35.0872	</td><td>6.79</td></tr>
						<tr><td>312</td><td>64.002</td><td>-27.833</td><td>199	</td><td>6.8717</td><td>35.0855	</td><td>6.43</td></tr>
						<tr><td>312</td><td>64.002</td><td>-27.833</td><td>254	</td><td>6.6958</td><td>35.0683	</td><td>6.42</td></tr>
						<tr><td>312</td><td>64.002</td><td>-27.833</td><td>354	</td><td>6.3275</td><td>35.031	</td><td>6.34</td></tr>
						<tr><td>312</td><td>64.002</td><td>-27.833</td><td>454	</td><td>5.9039</td><td>34.9862	</td><td>6.44</td></tr>
						<tr><td>312</td><td>64.002</td><td>-27.833</td><td>554	</td><td>5.7533</td><td>34.987	</td><td>6.38</td></tr>
						<tr><td>312</td><td>64.002</td><td>-27.833</td><td>844	</td><td>5.0649</td><td>34.9598	</td><td>6.13</td></tr>
						<tr><td>314</td><td>64.110</td><td>-29.000</td><td>51	</td><td>7.7994</td><td>35.0822	</td><td>6.91</td></tr>
						<tr><td>314</td><td>64.110</td><td>-29.000</td><td>403	</td><td>6.6015</td><td>35.0678	</td><td>6.46</td></tr>
						<tr><td>314</td><td>64.110</td><td>-29.000</td><td>707	</td><td>5.5014</td><td>34.976	</td><td>6.31</td></tr>
						<tr><td>314</td><td>64.110</td><td>-29.000</td><td>960	</td><td>4.633 </td><td>34.9474	</td><td>6.1 </td></tr>
						<tr><td>314</td><td>64.110</td><td>-29.000</td><td>1109	</td><td>4.1972</td><td>34.9435	</td><td>6.19</td></tr>
						<tr><td>314</td><td>64.110</td><td>-29.000</td><td>1417	</td><td>3.7364</td><td>34.9235	</td><td>6.38</td></tr>
						<tr><td>314</td><td>64.110</td><td>-29.000</td><td>1598	</td><td>3.3992</td><td>34.9006	</td><td>6.51</td></tr>
						<tr><td>315</td><td>64.132</td><td>-29.533</td><td>17	</td><td>8.6936</td><td>35.0759	</td><td>7.12</td></tr>
						<tr><td>315</td><td>64.132</td><td>-29.533</td><td>41	</td><td>7.8779</td><td>35.0814	</td><td>6.44</td></tr>
						<tr><td>315</td><td>64.132</td><td>-29.533</td><td>111	</td><td>7.0148</td><td>35.0911	</td><td>6.51</td></tr>
						<tr><td>315</td><td>64.132</td><td>-29.533</td><td>313	</td><td>6.5638</td><td>35.0706	</td><td>6.34</td></tr>
						<tr><td>315</td><td>64.132</td><td>-29.533</td><td>609	</td><td>5.5097</td><td>34.9747	</td><td>6.14</td></tr>
						<tr><td>315</td><td>64.132</td><td>-29.533</td><td>1011	</td><td>4.4229</td><td>34.9566	</td><td>6.27</td></tr>
						<tr><td>315</td><td>64.132</td><td>-29.533</td><td>1215	</td><td>3.9963</td><td>34.9411	</td><td>6.3 </td></tr>
						<tr><td>315</td><td>64.132</td><td>-29.533</td><td>1517	</td><td>3.4827</td><td>34.908	</td><td>6.49</td></tr>
						<tr><td>315</td><td>64.132</td><td>-29.533</td><td>1619	</td><td>3.4704</td><td>34.9063	</td><td>6.5 </td></tr>
					</table>
					<p>Other header columns that Java OceanAtlas 'understands' (but does not require) include CAST, BOTTOM (depth to bottom in meters), DATE (yyyymmdd format), and TIME (hhmm format).
						<br>
						<br> Java OceanAtlas will read any column of profile parameter data. For many common parameters, its internal lexicon helps Java OceanAtlas to interpret which of its standard parameters, for example those for which there are predefined color bars, is meant. But Java OceanAtlas will read any parameter, and even assign a name if the column heading (name) is more than four characters, though it is best for new parameters (e.g., concentration of a phytoplankton pigment) for users to supply a four character name in the column heading. Java OceanAtlas has many tools for making new and customized color bars, and for autoscaling contour plots, and so nearly any data will work. A small caveat is that it is best to avoid representing data values as very small (close to zero) numbers, e.g., 0.0003456. Such data often are best shown in columns pre-multiplied by a power of ten to bring their apparent numerical value - to Java OceanAtlas - away from zero. (This has to do with how computers handle arithmetic for very small numbers.)</p>
				</div>
			</div>
		</div>
		<div id="right" class="span4">
			<h1>Guided Tour of Java OceanAtlas</h1>
			<ul>
				<li><a href="basic_features.html">Basic Features</a></li>
				<li><a href="starting_joa.html">Starting JOA</a></li>
				<li><a href="station_maps.html">Station Maps</a></li>
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
				<li class="active"><a href="joa_data_files.html">Java OceanAtlas Data Files</a></li>
			</ul>
			<p><a class="cta-btn align-middle" href="joa.html">Explore</a></p>
		</div>
	</div>
</center>
