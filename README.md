# AlfattanKurniawan.github.io
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <title>Predicting Tobacco Sales to Youth in New York City • Nurvirta Monarizqa</title>
    
    <meta name="description" content="A project to predict whether a tobacco retailer in New York City will sell to youth and identify the variables that influence this activity using random forest, decision tree, bayesian networks, gaussian process, DBSCAN, and spatial autocorrelation.

"> 
    <meta name="keywords" content="">  	<!-- Twitter Cards -->
	<meta name="twitter:title" content="Predicting Tobacco Sales to Youth in New York City">
	<meta name="twitter:description" content="A project to predict whether a tobacco retailer in New York City will sell to youth and identify the variables that influence this activity using random forest, decision tree, bayesian networks, gaussian process, DBSCAN, and spatial autocorrelation.

">
	<meta name="twitter:site" content="@nmonarizqa">
	<meta name="twitter:creator" content="@nmonarizqa">
	
	<meta name="twitter:card" content="summary">
	<meta name="twitter:image" content="https://nmonarizqa.github.io/images/">
	
	<!-- Open Graph -->
	<meta property="og:locale" content="en">
	<meta property="og:type" content="article">
	<meta property="og:title" content="Predicting Tobacco Sales to Youth in New York City">
	<meta property="og:description" content="A project to predict whether a tobacco retailer in New York City will sell to youth and identify the variables that influence this activity using random forest, decision tree, bayesian networks, gaussian process, DBSCAN, and spatial autocorrelation.

">
	<meta property="og:url" content="https://nmonarizqa.github.io/portofolio/predicting-tobacco-sales-to-youth-nyc/">
	<meta property="og:site_name" content="Nurvirta Monarizqa">

    <link rel="canonical" href="https://nmonarizqa.github.io/portofolio/predicting-tobacco-sales-to-youth-nyc/">

    <link href="https://nmonarizqa.github.io/atom.xml" type="application/atom+xml" rel="alternate" title="Nurvirta Monarizqa Atom Feed">
    <link href="https://nmonarizqa.github.io/sitemap.xml" type="application/xml" rel="sitemap" title="Sitemap">

    <meta name="HandheldFriendly" content="True">
    <meta name="MobileOptimized" content="320">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="cleartype" content="on">

    <link rel="stylesheet" href="https://nmonarizqa.github.io/css/main.css">
    <!-- HTML5 Shiv and Media Query Support for IE -->
    <!--[if lt IE 9]>
      <script src="https://nmonarizqa.github.io/js/vendor/html5shiv.min.js"></script>
      <script src="https://nmonarizqa.github.io/js/vendor/respond.min.js"></script>
    <![endif]-->

</head>

<body id="js-body">
    <!--[if lt IE 9]><div class="upgrade notice-warning"><strong>Your browser is quite old!</strong> Why not <a href="http://whatbrowser.org/">upgrade to a newer one</a> to better enjoy this site?</div><![endif]-->
 <header id="masthead">
  <div class="inner-wrap">
    <a href="https://nmonarizqa.github.io/" class="site-title">Nurvirta Monarizqa</a>
    <nav role="navigation" class="menu top-menu">
        <ul class="menu-item">
	<li class="home"><a href="/">Nurvirta Monarizqa</a></li>
	
    
    <li><a href="https://nmonarizqa.github.io/portofolio/" >Portofolio</a></li>
  
    
    <li><a href="http://www.github.com/nmonarizqa" target="_blank">GitHub</a></li>
  
    
    <li><a href="http://www.medium.com/@nmonarizqa" target="_blank">Medium</a></li>
  
</ul>
    </nav>
  </div><!-- /.inner-wrap -->
</header><!-- /.masthead --> <nav role="navigation" id="js-menu" class="sliding-menu-content">
    <h5>Nurvirta Monarizqa <span>Table of Contents</span></h5>
    <ul class="menu-item">
         
        <li>
            <a href="https://nmonarizqa.github.io/portofolio/">
        <img src="https://nmonarizqa.github.io/images/portofolio.PNG" alt="teaser" class="teaser">
        <div class="title">Portofolio</div>
        <p class="excerpt">Things I’ve analyzed, designed, or developed.</p>
      </a>
        </li> 
        <li>
            <a href="http://www.github.com/nmonarizqa">
        
        <div class="title">GitHub</div>
        
      </a>
        </li> 
        <li>
            <a href="http://www.medium.com/@nmonarizqa">
        
        <div class="title">Medium</div>
        
      </a>
        </li>
    </ul>
</nav>
<button type="button" id="js-menu-trigger" class="sliding-menu-button lines-button x2" role="button" aria-label="Toggle Navigation">
  <span class="nav-lines"></span>
</button>

<div id="js-menu-screen" class="menu-screen"></div> 
    

    <div id="page-wrapper">
        <div id="main" role="main">
    <article class="wrap" itemscope itemtype="http://schema.org/Article">
         
  <nav class="breadcrumbs">
    <span itemscope itemtype="http://data-vocabulary.org/Breadcrumb">
      <a href="https://nmonarizqa.github.io" itemprop="url">
        <span itemprop="title">Home</span>
      </a> › 
    <span itemscope itemtype="http://data-vocabulary.org/Breadcrumb">
      <a href="https://nmonarizqa.github.io/portofolio/" itemprop="url">
        <span itemprop="title">Portofolio</span>
      </a>
    </span>
  </nav><!-- /.breadcrumbs -->

        <div class="page-title">
            <h1>Predicting Tobacco Sales to Youth in New York City</h1>
        </div>
        <div class="inner-wrap">
            <div id="content" class="page-content" itemprop="articleBody">
                <p><em>A project to predict whether a tobacco retailer in New York City will sell to youth and identify the variables that influence this activity using random forest, decision tree, bayesian networks, gaussian process, DBSCAN, and spatial autocorrelation.</em></p>

<p class="notice-inverse">
<strong>Authors</strong>: Nurvirta Monarizqa / Tashay Green / Zhaohong Niu / Sharon Jiaqian Liu. This is a final project for Machine Learning for Cities Course, CUSP New York University, Spring 2017.</p>

<h2 id="introduction">Introduction</h2>

<p>Roughly 260 million cigarettes were sold in the United States during 2016, contributing to over one trillion dollars in revenue for leading tobacco production companies. Most of the world’s tobacco is processed into cigarettes, however there is a growing market of other tobacco products such as smokeless tobacco, electronic cigarettes, hookahs, and others. The United States is the fourth largest tobacco-producing country in the world, whose citizens make up 16% of smokers across the globe. To reach the ~16% of smokers in the United States, tobacco companies spent over 10 billion dollars on marketing campaigns. Such ads have been known to specifically target women and adolescents; adolescents who find the ads appealing have an increased desire to begin smoking.</p>

<p>Cigarette smoking is common in adolescents ages 12 to 17. Many adult smokers report first trying smoking before the age of 18 as tobacco use is established primarily during adolescence. In New York City, 15,000 public high school students currently smoke cigarettes and will die prematurely as a result of smoking. Along with premature death, youth are at risk of developing lung diseases, cancers, and asthma from smoking.</p>

<p>Cigarette smoking among youth in the United States has declined in recent years but the use of other tobacco products has increased. Rates of electronic cigarette and hookah smoking have seen spikes among youth since 2011.</p>

<p>Because youth are most sensitive to the cost of tobacco products, making them less affordable has been an effective strategy for deterring consumption. Though cost increases are effective, other interventions such as stronger regulations are also necessary. Being able to determine the most vulnerable youth populations and environments, can significantly inform targeted reduction and regulation efforts.</p>

<h2 id="research-question-and-motivation">Research Question and Motivation</h2>

<p>The aim of this research project is to predict whether a tobacco retailer in New York City will sell to youth and identify the variables that influence this activity. This project has the potential to inform regulation policy and smoking reduction efforts relating to youth in New York City. Reducing smoking among youth in New York City may result in improved health conditions, social interactions,  and academic performance.</p>

<p>Determining whether and why a retailer may sell tobacco to youth is a challenging and imperfect science. Our interpretable models will be correlational and cannot pinpoint causality. Without detailed information about the lives of youth purchasing tobacco illegally (e.g., home location, socioeconomic status, guardianship status, school performance, etc.), it is impossible to definitively say how susceptible they may be to purchasing tobacco products. Furthermore, because reports of illegal sales to youth are initiated by citizens and not an enforcement agency, it is uncertain that the transaction actually occurred.</p>

<h2 id="related-work">Related Work</h2>

<p><strong>Analysis of factors related to illegal tobacco sales to young people in Ontario (O`Grady, Asbridge, Abernathy, 1999)</strong></p>

<p>Research conducted in Ontario, Canada concluded that older adolescents and females were more like to successfully purchase tobacco products, especially in tobacco-producing regions. Results of the study was gathered through random compliance checks of tobacco retailers where youth were intentionally sent to selected retailers to attempt a purchase of cigarettes.</p>

<p><strong>The density of tobacco retailers in home and school environments and relationship  with adolescent smoking behaviours in Scotland (Shortt, Tisch, Pearce, Richardson, Mitchell, 2016)</strong></p>

<p>This research project primarily sought to examine how the density of tobacco retailers impacted smoking rates among adolescents in Scotland. The study concluded that higher densities of tobacco retailers in residential neighborhoods, correlated with higher smoking rates in adolescents. A final recommendation was made to reduce density of neighborhood tobacco retailers to curb adolescent smoking.</p>

<p>We will apply prior thinking and research methodologies to the youth smoking endemic in New York City. Like the aforementioned related works, we have included variables for gender, age, retailer density, and retailer proximity to schools. Our research differs because we do not include the presence of tobacco production, use actual youth to solicit tobacco products, nor do we include information about youth younger than high school age. Referenced research does not make mention of using citizen reports of illegal sales during experimentation, which we will use in our iteration of research. Since the Ontario study relies on sparse compliance checks, our report data may be more telling since it can be obtained on a more frequent basis, as individuals are able to file reports any time.</p>

<h2 id="data">Data</h2>

<p><img src="https://nmonarizqa.github.io/images/tobacco-nyc.JPG" /></p>

<p>The dataset used in this project is a merged dataset from various resources (see Table 1). First, we got a dataset from New York State Open Data about the locations of all tobacco retailers in New York State. We spatially joined the data to a New York City shapefile to get only the tobacco retailers in New York City. Then, we filtered the 311 data to contain only reports pertaining to cigarette sales to youth. We merged both datasets based on location (nearest neighbor under 200 feet) to get the number of reports for each tobacco retailer.</p>

<p>Other factors that we are interested in are the proximity of the retailer to the subway station, distance to nearest high school, “density” of tobacco retailers and schools in a census tract. For the proximity, we calculated the distances of each tobacco retailer to the nearest subway and high school. For number of tobacco retailers, we spatially joined the census tract shapefile with tobacco retailer data. Lastly, for school density, we calculated the number of schools in a 1 mile radius of a given tobacco retailer.</p>

<p>To take into account socioeconomic and demographic factors, we gathered the total population and median household income of a census tract. We also retrieved academic performance data about high schools nearest tobacco retailers to paint a picture of the youth that may be illegally purchasing tobacco products. Academic data included the percentage of female students for a school, percentage of students for each race, enrollment, percent of poverty, and student achievement rating.</p>

<p>Finally, the master dataset contained 10526 tobacco retailers with 22 valid columns, including <code class="language-plaintext highlighter-rouge">id</code>, <code class="language-plaintext highlighter-rouge">BoroCT2010</code>, <code class="language-plaintext highlighter-rouge">n_report</code>,<code class="language-plaintext highlighter-rouge">DBN</code>, <code class="language-plaintext highlighter-rouge">school_distance</code>, <code class="language-plaintext highlighter-rouge">n_school</code>, <code class="language-plaintext highlighter-rouge">subway_distance</code>, <code class="language-plaintext highlighter-rouge">n_tobacco</code>, <code class="language-plaintext highlighter-rouge">Enrollment</code>, <code class="language-plaintext highlighter-rouge">Student Achievement Rating</code>, <code class="language-plaintext highlighter-rouge">Percent White</code>, <code class="language-plaintext highlighter-rouge">Percent Black</code>, <code class="language-plaintext highlighter-rouge">Percent Hispanic</code>, <code class="language-plaintext highlighter-rouge">Percent Asian</code>,<code class="language-plaintext highlighter-rouge">% Female</code>, <code class="language-plaintext highlighter-rouge">% Poverty</code>, <code class="language-plaintext highlighter-rouge">MHI</code>, <code class="language-plaintext highlighter-rouge">Total Population</code>, <code class="language-plaintext highlighter-rouge">type</code>, <code class="language-plaintext highlighter-rouge">latitude</code>, <code class="language-plaintext highlighter-rouge">longitude</code> and <code class="language-plaintext highlighter-rouge">class</code>.</p>

<p>Based on the feature <code class="language-plaintext highlighter-rouge">n_report</code>, which indicates the frequency of tobacco sales to youth, the whole dataset is split into classes. We did both binary class separations and multiclass separations of the data. For binary class separation, if the store had sold cigarettes to youth in the past, it was assigned to class 1, otherwise, 0. For multiclass separation, if the store had 0 reports, it was assigned to class 1, 1 to 2 reports it belong to class 2,  3 to 10 reports  it belong to class 3 and those contain more than 10 reports are class 4. Class information is stored in the feature <code class="language-plaintext highlighter-rouge">class</code> (see Table 2).</p>

<p><img src="https://nmonarizqa.github.io/images/table-2.JPG" /></p>

<p><cite><strong>Table 2.</strong>  <code class="language-plaintext highlighter-rouge">class</code> feature has been categorized in a binary and multiclass fashion based on the number of reports per tobacco retailer. Each machine learning method was attempted using binary and multiclass, typically only the binary classification produced fruitful results.</cite></p>

<p>Data Sources:</p>
<ul>
  <li><a href="https://health.data.ny.gov/Health/Active-Retail-Tobacco-Vendors/9ma3-vsuk/data">Tobacco Retailer NY</a></li>
  <li><a href="https://nycopendata.socrata.com/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9">311 reports</a></li>
  <li><a href="https://www.baruch.cuny.edu/confluence/display/geoportal/NYC+Mass+Transit+Spatial+Layers">Subway entrances</a></li>
  <li><a href="http://schools.nyc.gov/Accountability/data/GraduationDropoutReports/default.html">School performance data</a></li>
  <li><a href="http://data.beta.nyc/dataset/median-household-income-2010-census-tracts
http://www1.nyc.gov/site/planning/data-maps/nyc-population/census-2010.page">Median household income and population</a></li>
</ul>

<h2 id="methodologies">Methodologies</h2>
<h3 id="decision-tree">Decision Tree</h3>

<p>One classification method we utilized for this study was the Decision Tree. Using binary values as targets (0: never sold tobacco products to youth and 1: reportedly sold tobacco products to youth) for each tobacco retailer, we attempted to predict whether a retailer would or would not sell to youth.</p>

<p>In the first iteration, we trained a Decision Tree using attributes <code class="language-plaintext highlighter-rouge">school_distance</code>, <code class="language-plaintext highlighter-rouge">subway_distance</code>, <code class="language-plaintext highlighter-rouge">n_tobacco</code>, <code class="language-plaintext highlighter-rouge">Enrollment</code>, <code class="language-plaintext highlighter-rouge">Percent White</code>, <code class="language-plaintext highlighter-rouge">Percent Black</code>, <code class="language-plaintext highlighter-rouge">Percent Hispanic</code>, <code class="language-plaintext highlighter-rouge">Percent Asian</code>, <code class="language-plaintext highlighter-rouge">% Female</code>, <code class="language-plaintext highlighter-rouge">% Poverty</code>, <code class="language-plaintext highlighter-rouge">MHI</code>, and <code class="language-plaintext highlighter-rouge">Total Population</code>. The tree was able to predict targets with 84% accuracy, 57% precision, and 50% recall. Given that the model achieved 84% accuracy but lower values for precision and recall, we can assume that the decision tree actually predicted a fair number of targets incorrectly. To improve precision and recall we trained a second tree based on the important features identified by the initial tree.</p>

<p>A second decision tree was built using the important features <code class="language-plaintext highlighter-rouge">n_tobacco</code>, <code class="language-plaintext highlighter-rouge">MHI</code>,  <code class="language-plaintext highlighter-rouge">subway_distance</code>, <code class="language-plaintext highlighter-rouge">school_distance</code>, and <code class="language-plaintext highlighter-rouge">Total Population</code>. With the refined features, the model was able to predict targets with 84% accuracy, 71% precision, and 50% recall at max depth = 5 (see Figure 1).</p>

<p><img src="https://nmonarizqa.github.io/images/dt-tobacco.png" /></p>

<p><cite><strong>Figure 1.</strong> Decision tree based on the five important features of the data set, with max depth 5. The model predicted with 84% accuracy, whether a tobacco retailer would sell to youth, 71% precision and 50% recall. Illegal tobacco sales are of class 0 (no sale) and class 1 (has sold).</cite></p>

<p>Since this model did not take into account spatial attributes, we decided to use other methodologies to identify spatial autocorrelation.</p>

<h3 id="random-forest">Random Forest</h3>

<p>The random forest model is trained on the features <code class="language-plaintext highlighter-rouge">school_distance</code>, <code class="language-plaintext highlighter-rouge">n_school</code>, <code class="language-plaintext highlighter-rouge">subway_distance</code>, <code class="language-plaintext highlighter-rouge">n_tobacco</code>, <code class="language-plaintext highlighter-rouge">Enrollment</code>, <code class="language-plaintext highlighter-rouge">Student Achievement Rating</code>, <code class="language-plaintext highlighter-rouge">Percent White</code>, <code class="language-plaintext highlighter-rouge">Percent Black</code>, <code class="language-plaintext highlighter-rouge">Percent Hispanic</code>, <code class="language-plaintext highlighter-rouge">Percent Asian</code>, <code class="language-plaintext highlighter-rouge">% Female</code>, <code class="language-plaintext highlighter-rouge">% Poverty</code>, <code class="language-plaintext highlighter-rouge">MHI</code>, <code class="language-plaintext highlighter-rouge">Total Population</code>, <code class="language-plaintext highlighter-rouge">type</code>, <code class="language-plaintext highlighter-rouge">latitude</code> and <code class="language-plaintext highlighter-rouge">longitude</code> are used to fit the model. <code class="language-plaintext highlighter-rouge">Student Achievement Rating</code>, are categorized into multiclass and the feature <code class="language-plaintext highlighter-rouge">class</code> is the predictable multiclass (4 class) target.</p>

<p>After data preprocessing, the dataset is split into a training set and a testing set with 30/70 proportion. The random forest model successfully predicts 84.67% of the data. The precision is 21.16% and the recall is 25%. The low precision and recall are due to the use of multiclass classification as well as the existence of outliers in class 3 and class 4. The items of these two classes are highly random. The feature importance analysis states that median household income, total population and geographical position are top three factors which significantly impact the probability of tobacco sales to youth (see Table 3).</p>

<p><img src="https://nmonarizqa.github.io/images/table-3.JPG" /></p>

<p><cite><strong>Table 3.</strong> Random forest top 5 important features, <code class="language-plaintext highlighter-rouge">MHI</code>, <code class="language-plaintext highlighter-rouge">Total Population</code>, <code class="language-plaintext highlighter-rouge">longitude</code>, <code class="language-plaintext highlighter-rouge">n_tobacco</code>, and <code class="language-plaintext highlighter-rouge">latitude</code>.</cite></p>

<h3 id="bayesian-network">Bayesian Network</h3>

<p>We applied a Bayesian Network to classify the tobacco retailers, as well as look for anomalies within the data.The attributes used are <code class="language-plaintext highlighter-rouge">school_distance</code>, <code class="language-plaintext highlighter-rouge">n_school</code>, <code class="language-plaintext highlighter-rouge">subway_distance</code>, <code class="language-plaintext highlighter-rouge">n_tobacco</code>, <code class="language-plaintext highlighter-rouge">Enrollment</code>, <code class="language-plaintext highlighter-rouge">Student Achievement Rating</code>, <code class="language-plaintext highlighter-rouge">Percent White</code>, <code class="language-plaintext highlighter-rouge">Percent Black</code>, <code class="language-plaintext highlighter-rouge">Percent Hispanic</code>, <code class="language-plaintext highlighter-rouge">Percent Asian</code>, <code class="language-plaintext highlighter-rouge">% Female</code>, <code class="language-plaintext highlighter-rouge">% Poverty</code>, <code class="language-plaintext highlighter-rouge">MHI</code>, <code class="language-plaintext highlighter-rouge">Total Population</code>, <code class="language-plaintext highlighter-rouge">type</code>, <code class="language-plaintext highlighter-rouge">latitude</code> and <code class="language-plaintext highlighter-rouge">longitude</code>. Both binary and multiclass return the same best edges.</p>

<p>From the best edges, we know that some of these features have no relationship to our target class, so we remove them. The remaining features are <code class="language-plaintext highlighter-rouge">n_school</code>, <code class="language-plaintext highlighter-rouge">n_tobacco</code>, <code class="language-plaintext highlighter-rouge">MHI</code>, <code class="language-plaintext highlighter-rouge">Total Population</code>, <code class="language-plaintext highlighter-rouge">latitude</code> and <code class="language-plaintext highlighter-rouge">longitude</code>. Refer to Figure 3 for the network built by training the data.</p>

<p><img src="https://nmonarizqa.github.io/images/bayes-net.png" /></p>

<p><cite><strong>Figure 3.</strong> A visualization of the Bayesian network created by the training data. </cite></p>

<p>We tested this model ten times for both binary and multiclass. The model yields an average accuracy, precision, and recall of 84.67%, 42.4%, and 50% respectively for binary. The accuracy is good, however, the percentage of precision and recall are not as good, indicating that this model is good at predicting tobacco retailers that have never sold tobacco to youth, but not otherwise. For the multiclass, the model yields 85% of accuracy because all of the data records are predicted to be class 1. The model, when applied to multiclass, failed to detect classes other than class 1 (have never sold).</p>

<p>For the multiclass categorizations, we tried a different approach to detect the 6 data records belonging to class 4 (have sold &gt; 10). We applied the Bayesian network model above to catch anomalies. However, the top 10 elements with the least likelihood did not contain even 1 member of class 4. The model caught tobacco retailers that have sold tobacco to youth, but had abnormal attributes such as high median household income. Thus, we concluded that this model did not fit our data well.</p>

<p>Overall the model failed to detect multiclass record categorizations (and one of the multiclass as anomaly) most likely because elements in class 3 and 4 have rather random attributes and do not have any plausible pattern based on the attributes that we included in the model. Figure 4 shows that there is no specific spatial pattern for classes 3 and 4, so it is more difficult to detect them.</p>

<p><img src="https://nmonarizqa.github.io/images/dispersion.JPG" /></p>

<p><cite><strong>Figure 4.</strong>  Dispersion of tobacco retailers for multiclass categorizations of the target. Retailers that have 1-2 reports or 3-10 reports are more closely located than those with &gt;10 reports. </cite></p>

<h3 id="dbscan">DBSCAN</h3>

<p>To better understand the spatial distribution of tobacco retailers reported to have sold tobacco products to youth, we conducted DBSCAN and spatial autocorrelation analysis for anomaly detection and clustering.</p>

<p>We chose values where the number of points assigned to clusters were greater than 0 but less than 10% of the data, and scanned a wide range of parameter values. Using features <code class="language-plaintext highlighter-rouge">n_report</code>, <code class="language-plaintext highlighter-rouge">latitude</code> and <code class="language-plaintext highlighter-rouge">longitude</code>, the model detected an unusually dense area of retailers located in upper Manhattan. Figure 4 shows the results with parameters esp = 0.0015 and MinPts = 180 under a loop algorithm for DBSCAN analysis.</p>

<p>To cross-validate the result, we conducted spatial autocorrelation analysis (Moran’s I and hotspot analysis) to identify aggregated areas with a high number of reports. The dataset we used was the summed-up number of reports at the census tract level, with BoroCT Code attached to it. The attributes are transformed, spatial lag of number of reports, <code class="language-plaintext highlighter-rouge">number of reports</code> and <code class="language-plaintext highlighter-rouge">BoroCT Code</code> merged with census tract shapefile, and was shaped into row-standard with queen weight. The result of Local Moran’s I with Significant LISA (Local Indicator of Spatial Autocorrelation) is 0.167, while hotspot analysis with significant level set to 0.01 indicates that there is one major spatial correlation around East Harlem, Upper Manhattan (see Figure 6). The Moran’s I number is not as high as we expected, indicating that spatial distribution of reports could be rather random. Hotspot analysis supports our DBSCAN results that East Harlem of upper Manhattan has a higher density of reports.</p>

<h3 id="gaussian-process">Gaussian Process</h3>

<p>The gaussian process was used to predict the number of reports as a function of location. The attributes are the longitude and latitude, with the log of number of reports subtracted by the mean of all the logs, as the target. We used Gaussian Process Regressor with kernel equal to 0.185**2 * RBF(length_scale=0.01) + WhiteKernel(noise_level=0.49). We got the Logarithm of the Marginal Likelihood of -629.318. This number is greater than -1400, thus, the model is interpreted as being a good fit for the data. Much like the DBSCAN, the model is able to identify the cluster of retailers in upper Manhattan that have frequent occurrences of selling tobacco to youth.</p>

<p><img src="https://nmonarizqa.github.io/images/spatial.JPG" /></p>

<p><cite><em>Figure 4.</em>  Gaussian process, Spatial Autocorrelation, and DBSCAN show East Harlem, Manhattan as the most prevalent hotspot. </cite></p>

<h2 id="conclusion">Conclusion</h2>

<p>Of the predictive models used in this research, the model that best fit the data and yielded the greatest accuracy and precision values was the Decision Tree. The important features are: median household income, total population, number of tobacco retailers, distance to subway and distance to nearest high schools. According to the top five important features from our trained model (see Table 4),  the number of tobacco retailers within a census tract level has a significant impact on whether a retailer would sell cigarettes to youth. The spatial pattern we detected also indicates that East Harlem at Upper Manhattan is where a cluster of tobacco retailers are located that have reportedly sold to youth. Besides location attributes, demographics and socio-economic factors, especially income level of the community also plays an important role, as retailers located within areas of lower median household income are more prone to sell their tobacco products to youth.</p>

<table>
  <thead>
    <tr>
      <th>Variables</th>
      <th>Importance</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td># of tobacco retailers</td>
      <td>0.168881</td>
    </tr>
    <tr>
      <td>Median household income</td>
      <td>0.168077</td>
    </tr>
    <tr>
      <td>Distance to subway</td>
      <td>0.125977</td>
    </tr>
    <tr>
      <td>Distance to nearest high school</td>
      <td>0.0990679</td>
    </tr>
    <tr>
      <td>Total Population</td>
      <td>0.0625302</td>
    </tr>
  </tbody>
</table>

<p><cite><em>Table 4.</em> Feature importance for the Decision Tree</cite></p>

<p>The results of this study identify important socio-economic and spatial-related factors of tobacco retailers more inclined to sell cigarettes to youth.</p>

<h2 id="future-work">Future Work</h2>

<p>The 311 tobacco data is generated by residents who reported incidences of illegal sales. However, the propensity to call 311 might be different from one part of the city to another. In this project, we did not include that propensity as it is hard to obtain the exact numbers and the research are still ongoing. Also, it may be interesting to look at timeseries data and apply a model that counts recency and frequency as the attributes, as well as other external attributes such as tobacco survey to youth, tobacco advertisements, etc. to create a model that better predict multiclass targets for tobacco retailers that are likely to sell tobacco to youth.</p>

<h2 id="references">References</h2>

<ul>
  <li>
    <p>Richardson L, Hemsing N, Greaves L, et al. Preventing Smoking in Young People: A Systematic Review of the Impact of Access Interventions. International Journal of Environmental Research and Public Health. 2009;6(4):1485-1514. Retrieved from 10.3390/ijerph6041485</p>
  </li>
  <li>
    <p>Board on Population Health and Public Health Practice; Institute of Medicine; Bonnie RJ, Stratton K, Kwan LY, editors. Public Health Implications of Raising the Minimum Age of Legal Access to Tobacco Products. Committee on the Public Health Implications of Raising the Minimum Age for Purchasing Tobacco Products. 2015 Jul 23. 6, Retrieved from: https://www.ncbi.nlm.nih.gov/books/NBK310405/</p>
  </li>
  <li>
    <p>O’Grady B, Asbridge M, Abernathy T.  Analysis of factors related to illegal tobacco sales to young people in Ontario Tobacco Control 1999;8:301-305. Retrieved from: http://tobaccocontrol.bmj.com/content/8/3/301</p>
  </li>
</ul>

<p><a href="https://github.com/nmonarizqa/tobacco-nyc">Github</a></p>

                <hr />
                <footer class="page-footer">
                    

<div class="author-image">
	<img src="https://nmonarizqa.github.io/images/bio-photo.jpg" alt="Nurvirta Monarizqa">
</div><!-- ./author-image -->
<div class="author-content">
	<h3 class="author-name" >Written by <span itemprop="author">Nurvirta Monarizqa</span></h3>
	<p class="author-bio">Urban, Data, Visualization, and everything in between.</p>
</div><!-- ./author-content --> <div class="inline-btn">
	<a class="btn-social twitter" href="https://twitter.com/intent/tweet?text=Predicting%20Tobacco%20Sales%20to%20Youth%20in%20New%20York%20City&amp;url=https://nmonarizqa.github.io/portofolio/predicting-tobacco-sales-to-youth-nyc/&amp;via=nmonarizqa" target="_blank"><i class="fa fa-twitter" aria-hidden="true"></i> Share on Twitter</a>
	<a class="btn-social facebook" href="https://www.facebook.com/sharer/sharer.php?u=https://nmonarizqa.github.io/portofolio/predicting-tobacco-sales-to-youth-nyc/" target="_blank"><i class="fa fa-facebook" aria-hidden="true"></i> Share on Facebook</a>
	<a class="btn-social google-plus"  href="https://plus.google.com/share?url=https://nmonarizqa.github.io/portofolio/predicting-tobacco-sales-to-youth-nyc/" target="_blank"><i class="fa fa-google-plus" aria-hidden="true"></i> Share on Google+</a>
</div><!-- /.share-this -->
 <div class="page-meta">
	<p>Updated <time datetime="2017-07-10T11:29:57Z" itemprop="dateModified">July 10, 2017</time>
</div><!-- /.page-meta -->
                </footer>
                <!-- /.footer -->
                <aside>
                    
                </aside>
            </div>
            <!-- /.content -->
        </div>
        <!-- /.inner-wrap -->
        
    </article>
    <!-- ./wrap -->
</div>
<!-- /#main -->
 <footer role="contentinfo" id="site-footer">
	<nav role="navigation" class="menu bottom-menu">
		<ul class="menu-item">
		
      
			<li><a href="https://www.linkedin.com/in/nmonarizqa" target="_blank">LinkedIn</a></li>
		
      
			<li><a href="http://www.medium.com/@nmonarizqa" target="_blank">Medium</a></li>
		
		</ul>
	</nav><!-- /.bottom-menu -->
	<p class="copyright">&#169; 2021 <a href="https://nmonarizqa.github.io">Nurvirta Monarizqa</a> powered by <a href="http://jekyllrb.com" rel="nofollow">Jekyll</a> + <a href="http://mmistakes.github.io/skinny-bones-jekyll/" rel="nofollow">Skinny Bones</a>.</p>
</footer>
    </div>


    <script src="https://nmonarizqa.github.io/js/vendor/jquery-1.9.1.min.js"></script>
    <script src="https://nmonarizqa.github.io/js/main.js"></script>

</body>

</html>
