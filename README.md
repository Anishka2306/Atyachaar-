<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">  
  <meta name="viewport" content="width=device-width, initial-scale=1.0">  
  <title>Women Safety Statistics Dashboard - India (2020-2025)</title>  
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>  
  <link rel="stylesheet" href="style.css"> <!-- External CSS link -->
</head>  
<body>  
  <div class="container">  
    <!-- Header Section -->
    <div class="header">  
      <h1>Women Safety Statistics Dashboard</h1>  
      <p>Crime Statistics Against Women in India (2020-2025)</p>  
    </div>  

    <!-- Filters -->
    <div class="filters">  
      <div class="filter-row">  
        <div class="filter-group">  
          <label for="yearSelect">Year</label>  
          <select id="yearSelect">  
            <option value="2024">2024</option>  
            <option value="2023">2023</option>  
            <option value="2022">2022</option>  
            <option value="2021">2021</option>  
            <option value="2020">2020</option>  
          </select>  
        </div>  
        <div class="filter-group">  
          <label for="stateSelect">State</label>  
          <select id="stateSelect">  
            <option value="all">All States</option>  
            <option value="uttar-pradesh">Uttar Pradesh</option>  
            <option value="maharashtra">Maharashtra</option>  
            <option value="west-bengal">West Bengal</option>  
            <option value="rajasthan">Rajasthan</option>  
            <option value="bihar">Bihar</option>  
            <option value="madhya-pradesh">Madhya Pradesh</option>  
            <option value="delhi">Delhi</option>  
            <option value="karnataka">Karnataka</option>  
          </select>  
        </div>  
        <div class="filter-group">  
          <label for="crimeType">Crime Type</label>  
          <select id="crimeType">  
            <option value="all">All Crimes</option>  
            <option value="rape">Rape Cases</option>  
            <option value="dowry">Dowry Deaths</option>  
            <option value="murder">Murder Cases</option>  
          </select>  
        </div>  
        <div class="filter-group">  
          <label>&nbsp;</label>  
          <button onclick="updateDashboard()">Update Dashboard</button>  
        </div>  
      </div>  
    </div>  

    <!-- Stats Cards -->
    <div class="stats-grid">  
      <div class="stat-card">  
        <div class="stat-number rape-cases" id="rapeTotal">28,046</div>  
        <div class="stat-label">Rape Cases (2024)</div>  
      </div>  
      <div class="stat-card">  
        <div class="stat-number dowry-cases" id="dowryTotal">6,589</div>  
        <div class="stat-label">Dowry Deaths (2024)</div>  
      </div>  
      <div class="stat-card">  
        <div class="stat-number murder-cases" id="murderTotal">4,932</div>  
        <div class="stat-label">Murder Cases (2024)</div>  
      </div>  
      <div class="stat-card">  
        <div class="stat-number total-cases" id="totalCases">39,567</div>  
        <div class="stat-label">Total Cases (2024)</div>  
      </div>  
    </div>  

    <!-- Charts -->
    <div class="dashboard">  
      <div class="chart-container">  
        <div class="chart-title">Crime Statistics by State</div>  
        <canvas id="stateChart"></canvas>  
      </div>  
      <div class="chart-container">  
        <div class="chart-title">Yearly Trend Analysis</div>  
        <canvas id="trendChart"></canvas>  
      </div>  
      <div class="chart-container">  
        <div class="chart-title">Crime Type Distribution</div>  
        <canvas id="pieChart"></canvas>  
      </div>  
      <div class="chart-container">  
        <div class="chart-title">Top 10 Cities by Crime Rate</div>  
        <canvas id="cityChart"></canvas>  
      </div>  
    </div>  

    <!-- Data Table -->
    <div class="data-table">  
      <table id="dataTable">  
        <thead>  
          <tr>  
            <th>State/City</th>  
            <th>Rape Cases</th>  
            <th>Dowry Deaths</th>  
            <th>Murder Cases</th>  
            <th>Total Cases</th>  
            <th>Rate per 100k</th>  
          </tr>  
        </thead>  
        <tbody id="tableBody"></tbody>  
      </table>  
    </div>  

    <!-- Disclaimer -->
    <div class="disclaimer">  
      <h3>Important Note</h3>  
      <p><strong>Demo Data:</strong> This dashboard uses simulated statistical data for demonstration purposes. The actual crime statistics should be obtained from official sources like NCRB, Ministry of Home Affairs, Govt. of India.</p>  
    </div>  
  </div>  

  <script src="script.js"></script> <!-- External JS file -->
</body>  
</html># Atyachaar-
