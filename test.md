---
layout: page
title: Milanfx Study Notes
permalink: /xxx/
---


# Implementing Data Modeling in Tableau

<p>Estimated time needed: <strong>15</strong> minutes.</p>
<p>In this lab, you will learn how to implement data modeling in
Tableau.</p>
<h2 id="required-software">Required Software</h2>
<p>You can complete this lab using the free, downloadable
<strong>Tableau Desktop (Public Edition)</strong> desktop software. You
may also use the free <strong>Tableau Public online platform</strong>,
but some tasks may not work in exactly the same way or may not be
supported in that version.</p>
<h2 id="prerequisites">Prerequisites</h2>
<p>You need a free Tableau Public account for this lab. If you haven't
already done so, you can sign up for an account using the steps
<a href="https://ske-200666-getting-started-with-tableau-sk228091-13e06c0574350f.gitlab.io/labs/v1/m1/Sign%20Up%20for%20Tableau%20Public.md.html" target="_blank">here</a>.</p>
<p><strong><em>Disclaimer: The screenshots in this lab are taken from
Tableau Desktop. If you are using Tableau Public, you may notice some
differences due to version variations.</em></strong></p>
<h2 id="data-set">Data Set</h2>
<p>This lab uses several sample data sets called
<strong>Country.csv</strong>, <strong>Indicators_small.csv</strong>, and
<strong>Series.csv</strong> to showcase the Tableau features used in
these lab exercises.</p>
<p>Hold the CTRL key while you click to download each of the following
files:</p>
<p><a href="data/Country.csv">Country.csv</a></p>
<p><a href="data/Indicators_small.csv">Indicators_small.csv</a></p>
<p><a href="data/Series.csv">Series.csv</a></p>
<h2 id="objectives">Objectives</h2>
<p>The exercises in this lab teach you how to implement data modeling in
Tableau</p>
<p>In this hands-on lab, you will:</p>
<ol type="1">
<li>Implement data modeling</li>
</ol>
<h1 id="exercise-implement-data-modeling">Exercise: Implement Data
Modeling</h1>
<p>In this exercise, you will learn how to join tables by joining the
<strong>Country</strong> table with the
<strong>Indicators_small</strong> table.</p>
<ol type="1">
<li>Under <strong>To a File</strong>, click <strong>Text
file</strong>.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/To_a_File_Text.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="2" type="1">
<li>Navigate to the folder where you downloaded the data sets to, then
select <strong>Country.csv</strong>, and click
<strong>Open</strong>.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Country_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="3" type="1">
<li>Right-click <strong>Country.csv</strong> and click
<strong>Open</strong>. You are now viewing the physical table that
defines the logical table of the same name. You need to view the
physical table as joins are done between physical tables, not logical
tables.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Open_Country.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="4" type="1">
<li>Drag <strong>Indicators_small.csv</strong> to the right of
<strong>Country.csv</strong>.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Join_Country_Indicators_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="5" type="1">
<li><p>Click the <strong>Inner Join</strong> symbol.</p></li>
<li><p>You can see these two tables are now part of an <em>Inner
Join</em>, and you can see the four types of join (Inner, Left, Right,
and Full Outer). The common field in this join is <em>Country
Code</em>.</p></li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Join_Country_Indicators_2.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="7" type="1">
<li><p>Close the <strong>Join</strong> window.</p></li>
<li><p>You'll now join the <em>Indicators_small</em> table with the
<em>Series</em> table, by dragging <strong>Series.csv</strong> to the
right of <strong>Indicators_small.csv</strong>.</p></li>
<li><p>Click the <strong>Inner Join</strong> symbol.</p></li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Join_Indicators_Series_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="10" type="1">
<li>You can see these two tables are now part of another <em>Inner
Join</em>, and you can see that the common field in this join is
<em>Indicator Name</em>.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Join_Indicators_Series_2.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="11" type="1">
<li><p>Close the <strong>Join</strong> window and click
<strong>X</strong> in the top right corner of the canvas.</p></li>
<li><p>Hover over the <strong>Country.csv</strong> data file.</p></li>
<li><p>You can see that Country.csv is one logical table combined with
three physical tables: Country.csv, Indicators_small.csv, and
Series.csv.</p></li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Join_Indicators_Series_3.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="14" type="1">
<li>Click the little arrow to the right of <strong>Country.csv</strong>
and click Remove.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Join_Indicators_Series_4.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<p>Having created joins, you will now create a relationship between two
logical tables.</p>
<ol start="15" type="1">
<li><p>Drag the <strong>Country.csv</strong> dimension to the canvas
area.</p></li>
<li><p>Drag <strong>Indicators_small.csv</strong> in the canvas area
just next to <strong>Country.csv</strong>.</p></li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Relationship_Country_Indicators_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="17" type="1">
<li><p>Hover over the orange line (the noodle) joining
<strong>Country.csv</strong> and
<strong>Indicators_small.csv</strong>.</p></li>
<li><p>You can see that the relationship type (or <em>Cardinality</em>)
is the default <em>Many to Many</em> relationship, and the common (or
<em>Related</em>) field is <em>Country Code</em>.</p></li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Relationship_Country_Indicators_2.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="19" type="1">
<li>In the bottom-left of the canvas, expand <strong>Performance
Options</strong>; in <strong>Cardinality</strong>, select
<strong>One</strong> from the first drop-down list.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Relationship_Country_Indicators_3.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="20" type="1">
<li><p>Hover over the noodle joining <strong>Country.csv</strong> and
<strong>Indicators_small.csv</strong>.</p></li>
<li><p>You can see that this relationship is now a <em>One-to-many</em>
relationship.</p></li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Relationship_Country_Indicators_4.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<p>Now that you've created a join and a relationship between two or more
tables, next, you'll visualize the data for presentation.</p>
<ol start="22" type="1">
<li>In the data window, click <strong>Update Now</strong>.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Update_now.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="23" type="1">
<li>Click the <strong>Sheet 1</strong> worksheet tab to extract the
data.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Sheet1.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="24" type="1">
<li><p>Drag <strong>Region</strong> to <strong>Rows</strong>.</p></li>
<li><p>Click the right arrow of the <strong>Region</strong> pill and
select <strong>Filter</strong>.</p></li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Region_filter_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="26" type="1">
<li>Uncheck <strong>Null</strong> in the list and click
<strong>OK</strong>.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Region_filter_2.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="27" type="1">
<li>This removes Null from the visualization table.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Region_filter_3.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="28" type="1">
<li>From the <strong>Indicators_small.csv</strong> table in the
<strong>Data</strong> pane on the left, drag <strong>Country
Name</strong> to <strong>Rows</strong>.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Population_census_1.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="29" type="1">
<li>Drag the <strong>Latest Population Census</strong> measure to
<strong>Columns</strong>.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Population_census_2.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="30" type="1">
<li>Click on the right arrow of the <strong>Latest Population
Census</strong> pill and select <strong>Filter</strong>.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Population_census_3.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="31" type="1">
<li><p>On the <strong>Filter</strong> tab, ensure that <strong>Include
Null Values</strong> is unchecked.</p></li>
<li><p>Click <strong>OK</strong>.</p></li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Population_census_4.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<ol start="33" type="1">
<li>You now have a bar chart visualization of each country's Latest
Population Census year.</li>
</ol>
<div style="display: inline-grid; border: 3px solid var(--word); margin:10px 0px;"><img src="https://ske-200668-advanced-data-visualization-with-tabl-b07ed2d9623e6b.gitlab.io/labs/v1/m1/images/Population_census_5.png" style="width:880px; max-height:500px; object-fit:contain;"></div>
</p>
<h3
id="congratulations-you-have-completed-this-lab-and-are-ready-for-the-next-topic.">Congratulations!
You have completed this lab and are ready for the next topic.</h3>




