---
layout : datapage
title : Arctic Datapage
ocean: Arctic
---

<section id="hero">
	<div class="hero-container">
		<h1>Explore {{page.ocean}} Ocean Data</h1>
		<h2>Navigate to your desired data below</h2>
		<!--# <center style="color: white; padding: 1%;"><a class='button-func' href="#tree-search"> Tree Search </a></center> -->
		<center><img src="assets/images/Arctic_map.jpg" alt="" class="responsive" style="width:100%"></center>
	</div>
</section>
<!-- #hero -->
<section id="call-to-action1">
	<section id="call-to-action3">
		<div class="container wow fadeIn">
			<div class="col-lg-9 text-center text-lg-left" style="flex:0 0 100%;max-width:100%">
				<h3 class="cta-title1" style="text-align:center">About {{page.ocean}} Ocean Data</h3>
				<br>
				<p class="cta-text1" style="text-align:center">Vertical section data from Arctic Ocean and Nordic Seas expeditions from J. Swift's files. The data values for measured parameters are unchanged (with one exception), but the files have been vetted and groomed for improved readability and consistency, and assembled in sensible geographic order.</p>
			</div>
		</div>
	</section>
</section>
<!-- #call-to-action -->
<div style="background-color: black">
		<div class="container h-100">
			<center style="color: white;font-size: 25px;font-family: 'Poppins';margin-top: 7%;"> Pick a Search Functionality</center>
			<center style="color: white; padding-top: 5%;"><a class='button-func' href="#tree-search"> Tree Search </a>
			<a class='button-func' href="#dropdown-search"> Dropdown Search </a></center>
			<hr class="style-one">
			<center style="color: white;font-size: 25px;font-family: 'Poppins';margin-top: 7%;"> Dropdown Search</center>
			<section id="dropdown-search">
			<div class="row h-100 align-items-center justify-content-center">
				<div class="col-12 col-md-10">
					<div class="hero-search-form">
						<div class="tab-content" id="nav-tabContent">
							<div class="tab-pane fade show active" id="nav-places" role="tabpanel" aria-labelledby="nav-places-tab">
								<h6>What data are you looking for?</h6>
								<div class="row">
									<div class="mx-auto">
									<form style="margin-left: auto;" action="#" method="get">
											<select class="custom-select" id="verticalSectionDropdown">
												<option value="All" selected="selected">Section</option> {% for item in site.data.arcticdata.section%}
												{% if item.diff[0]%}
												<option value="{{item.title}}">{{item.title}}</option>
												{% else %}
												{% for entry in item.years%}
												<option value="{{entry.year}}">{{entry.year}}</option> {% endfor %} {% endif%} 
												{% endfor %} 
											</select> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;


											<select style="display:none" class="custom-select" id="yearDropdown">
												<option value="All">Year</option> {% for item in site.data.arcticdata.yeardropdown %}
												<option value="{{item.year}}">{{item.year}}</option> {% endfor %} </select> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
											<select style="display:none" class="custom-select" id="fileDropdown">
												<option value="All">File</option>
												<option value="Basin">.csv</option>
												<option value="Sub Basin">.jos</option>
												<option value="Option_3">.txt</option>
												<option value="Option_4">.joa</option>
												<option value="Option_5">.zip</option>
											</select>
									</form>
									</div>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
			</section>
		</div>
			<div class="container-table100">
				<div class="wrap-table100">
					<div class="table100 ver3 m-b-110" style="padding-top:60px;">
						<div class="table100-head">
							<table>
								<thead>
									<tr class="row100 head">
										<th class="cell100 column1">Section</th>
										<th class="cell100 column4">File</th>
									</tr>
								</thead>
							</table>
						</div>
						<div class="table100-body js-pscroll" style="max-height:1500px">
							<table class="table" id="datatable1">
								<tbody id="datatable"> {% for item in site.data.arcticdata.section%} 
								{% if item.diff[0]%}
								{% for entry in item.diff%}
								<tr>
										<td class="cell100 column1">{{item.title}}</td>
										<td class="cell100 column4"><a href="{{entry.path}}">{{entry.name}}</a></td>
								</tr>
								{% endfor %}
								{% else %}
								{% for entry in item.years%}{% for file in entry.files%}
									<tr>
										<td class="cell100 column1">{{entry.year}}</td>
										<td class="cell100 column4"><a href="{{file.path}}">{{file.name}}</a></td>
									</tr> {% endfor %} {% endfor %} {% endif %}
								{% endfor %}</tbody>
							</table>
						</div>
					</div>
				</div>
			</div>
	<hr class="style-two">
	<center style="color: white;font-size: 25px;padding-bottom: 3%;font-family: 'Poppins';"> Data Tree Search</center>
	<section id="tree-search">
	<div class="tree ">
			<ul> <span style="color:white;font-size: 20px;"><b>{{page.ocean}} Ocean</b></span>
				<ul>
					<li> <span style="background:#5cb85c;color:white">Download all {{page.ocean}} Data</span></li>
					<li><a href="assets/documents/Guide to the Best Data Arctic directory.pdf"><span style="color:white">Guide to Arctic Ocean and Nordic Sea files</span></a></li>
					{% for item in site.data.arcticdata.section %}
					<li> <span style="color:white"><i class="fa fa-plus-square" style="color:white"></i>{{item.title}}</span>
						<ul>
								{% if item.diff[0]%}
								{% for entry in item.diff%}
							    <li><span style="color:white"><a href="{{entry.path}}">{{entry.name}}</a></span></li>
								{% endfor %}
								{% else %}
								{% for entry in item.years%}
								<li> <span style="color:white"><i class="fa fa-plus-square" style="color:white"></i>{{entry.year}}</span>
								<ul> {% for file in entry.files%}
								<li><span style="color:white"><a href="{{file.path}}">{{file.name}}</a></span></li> {% endfor %} </ul>
								</li> 
								{% endfor %} 
								{% endif %}
						</ul> 
					</li> {% endfor %} 
				</ul>
			</ul>
	</div>
	</section>
</div>
