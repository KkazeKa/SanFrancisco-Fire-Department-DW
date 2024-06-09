<h2>San Francisco fire department Dw</h2>
<h3>This Project was conducted using SQL server data tools stack (SSIS , SSAS)</h3>

<h3>Business Process:</h3>
<p>The Fire Incident Analysis project aims to analyze data collected by the San Francisco Fire Department to improve operational efficiency and performance. The process involves data collection, transformation, modeling, analysis, and performance improvement strategies based on derived insights.</p>


<h3>Data description</h3>
<p>The dataset under analysis contains detailed information on fire incidents responded to by the San Francisco Fire Department. Each incident record provides a comprehensive summary, including incident date, incident number, call number, alarm date, and arrival date. This report aims to provide a thorough analysis of the dataset to derive actionable insights and enhance operational efficiency.</p>
<img src='https://github.com/KkazeKa/SanFrancisco-Fire-Department-DW/assets/87916759/61d0b9e2-9a17-48b9-b00e-b1728794f394'>





<h3>Problematic :</h3>
<img src='https://github.com/KkazeKa/SanFrancisco-Fire-Department-DW/blob/main/sfdw.jpeg?raw=true' >

<h3>Granularity</h3>
<p>In this project, the granularity is at the level of individual fire incidents.
Each fire incident record contains details such as incident date, incident number, call number, alarm date, arrival date, primary situation, action taken, Unit Type responding, etc.</p>

<h3>Dimensions</h3>
<div>
        <h4>a. Time Dimension</h4>
        <p>
            Captures temporal aspects such as incident date, alarm time, and arrival time.
            Enables analysis of incident trends over different time periods, facilitating insights into seasonal variations and daily patterns of emergency calls.
        </p>
</div>
    <div>
        <h4 class="location">b. Location Dimension</h4> <!-- Changed to h4 with location class -->
        <p>
            Provides geographical information about incident locations, including address, district, and coordinates.
            Facilitates spatial analysis to identify high-incidence areas, assess response coverage, and optimize resource allocation based on geographic distribution.
        </p>
    </div>
    <div>
        <h4>c. Incident Dimension</h4>
        <p>
            Describes the nature and type of each incident, including primary situation and action taken.
            Allows for categorization and analysis of incident types to identify common scenarios, prioritize response protocols, and assess the effectiveness of actions taken.
        </p>
    </div>
    <div>
        <h4>d. Unit Dimension</h4>
        <p>
            Represents the units or resources deployed in response to each incident, such as fire engines, ambulances, and personnel.
            Enables analysis of resource utilization, response team performance, and workload distribution across different units.
        </p>
    </div>


<h3>Business Questions and KPIs</h3>
    
 <ul>
        <li>KPI: Calculate the average response time for incidents on a yearly basis.</li>
        <li>Determine the number of calls received each year.</li>
        <li>Identify the neighbourhoods with the highest number of incidents.</li>
    </ul>

<h3>Steps:</h3>

<ul>
    <li>Load Data from csv file ( Bulk Load)</li>
    <li>Create datawarehouse followig a star schema model</li>
    <li>Load Data into a ssas cube for multidimensionnal querying</li>
    
</ul>
  
  
