# Project: NYRR Race Data
<b>Question: How did COVID impact NYRR races?</b><br><br>
Tableau Dashboard<br>
Tableau Story Presentation<br>

Data Created:
June 2023

## Project Summary

New York Road Runners (NYRR) is the largest race organizer in New York City. They host dozens of races every year, including the world-famous New York City Marathon every November. For this project, I scraped ten years of race data from their race results website; the data includes the name, date, location, distance, and runner demographics of each race they've hosted since 2014.

I was interested in exploring this dataset because I hypothesized (based on my own experience) that more New Yorkers picked up running as a hobby during COVID. I wanted to understand how NYRR's race portfolio has evolved in the past decade and how COVID impacted their race participation.

## Process
<b>Data Source:</b> <a href="https://results.nyrr.org/home">NYRR Race Results website</a> (data scraped in June 2023, using the Google Chrome extension Webscraper.io)<br>
<br>
<b>Data Limitations:</b><br>
	• The dataset only covers June 2014 - June 2023, because NYRR only displays race data from the past ten years on their website. <br>
	• The dataset lacks personally identifiable information about the runners. There is no way to determine how many new or returning runners are encapsulated in the <em>totalrunners</em> cell for each race. <br>
 <br>
<b>Data Cleanup & Preparation:</b><br>
	• I removed races from 2014 & 2023 from the dataset, since the data from those years is incomplete.<br>
	• In the <em>location</em> column, I merged similar locations (e.g. "Coney Island, Brooklyn" and "Coney Island").<br>
	• I created and populated the <em>borough</em> column, identifying the borough each race took place in.<br>
	• I created and populated the <em>distance.miles</em> column. The original <em>distance</em> column has a mix of distances in miles & kilometers, while the <em>distance.miles</em> column has all of the race distances converted to miles, to allow for direct distance comparision between races. <br>
	• I created and populated a <em>status</em> column, identifying which races were virtual and which races were in-person. <br>


