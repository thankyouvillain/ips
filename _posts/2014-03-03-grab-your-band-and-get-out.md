---
date: 2017-05-11 12:00:00
layout: post
title: Film_History
subtitle: Lorem ipsum dolor sit amet, consectetur adipisicing elit.
description: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
image: https://upload.wikimedia.org/wikipedia/en/0/0b/The_Man_Standing_Next_movie_poster%2C_Jan_2020.jpg
optimized_image: https://upload.wikimedia.org/wikipedia/en/0/0b/The_Man_Standing_Next_movie_poster%2C_Jan_2020.jpg
category: music
tags:
  - music
  - band
  - passion
author: thiagorossener
---

<html>

    <script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>
          <script type="text/javascript">
            google.charts.load("current", {packages:["timeline"]});
            google.charts.setOnLoadCallback(drawChart);
            function drawChart() {
          
              var container = document.getElementById('example3.1');
              var chart = new google.visualization.Timeline(container);
              var dataTable = new google.visualization.DataTable();
              dataTable.addColumn({ type: 'string', id: 'Room' });
              dataTable.addColumn({ type: 'string', id: 'Name' });
              dataTable.addColumn({ type: 'date', id: 'Start' });
              dataTable.addColumn({ type: 'date', id: 'End' });
              dataTable.addRows([
                [ 'Korea', 'Jeong Do-jeon&Six Flying Dragons',       new Date(1374,12,0,0,0,0),  new Date(1398,8,0,0,0,24) ],
                [ 'Korea', 'The Fortress',       new Date(1637,1,3,0,0,0),  new Date(1637,2,24,0,0,24) ],
                [ 'Korea', '1987',       new Date(1987,1,14,0,0,0),  new Date(1987,7,5,0,0,0) ],
                [ 'Korea', 'Default',       new Date(1997,1,23,0,0,0),  new Date(1997,12,6,0,0,0) ],
                [ 'Korea', 'Present',    new Date(2022,1,0,0,0,0),  new Date(2022,2,0,0,0,0) ],
                ]);
          
              var options = {
                timeline: { colorByRowLabel: true }
              };
          
              chart.draw(dataTable, options);
            }
          
          </script>
    
    <div id="example4.1" ></div>
    <div id="example5.1" ></div>
    <div id="example3.1"></div>
</html>

<html>
<head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<script>
$(document).ready(function(){
  $("#myInput").on("keyup", function() {
    var value = $(this).val().toLowerCase();
    $("#myTable tr").filter(function() {
      $(this).toggle($(this).text().toLowerCase().indexOf(value) > -1)
    });
  });
});

function sortTable(n) {
  var table, rows, switching, i, x, y, shouldSwitch, dir, switchcount = 0;
  table = document.getElementById("myTable");
  switching = true;
  dir = "asc"; 
  while (switching) {
    switching = false;
    rows = table.rows;
    for (i = 0; i < (rows.length - 1); i++) {
      shouldSwitch = false;
      x = rows[i].getElementsByTagName("TD")[n];
      y = rows[i + 1].getElementsByTagName("TD")[n];
      if (dir == "asc") {
        if (x.innerHTML.toLowerCase() > y.innerHTML.toLowerCase()) {
          shouldSwitch= true;
          break;
        }
      } else if (dir == "desc") {
        if (x.innerHTML.toLowerCase() < y.innerHTML.toLowerCase()) {
          shouldSwitch = true;
          break;
        }
      }
    }
    if (shouldSwitch) {
      rows[i].parentNode.insertBefore(rows[i + 1], rows[i]);
      switching = true;
      switchcount ++;      
    } else {
      if (switchcount == 0 && dir == "asc") {
        dir = "desc";
        switching = true;
      }
    }
  }
}
</script>
<style>
table {
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width: 100%;
  font-size:4vw;
}

td, th {
  border: 1px solid #dddddd;
  text-align: center;
  padding: 1px;
}

th {
  background-color: #041a4f;
  cursor: pointer;
  color: white;
  position: sticky;
  top: 0; 
  box-shadow: 0 2px 2px -1px rgba(0, 0, 0, 0.4);
}

th:hover {
    background-color:#04AA6D;
    color: white;    

  }

td{
    border: 2px solid #000000;
  }

tr:nth-child(even) {
  background-color: #dddddd;
}
  
tr:hover {
    background-color:#04AA6D;
    color: white;      
}
</style>
</head>
<body>

<p>Film_History</p>
<input id="myInput" type="text" placeholder="Search">
<br><br>

<table>
  <thead>
  <tr>
    <th onclick="sortTable(0)">Year <i class="fa fa-sort"></i></th> 
    <th onclick="sortTable(1)">Title<i class="fa fa-sort"></i></th> 
    <th onclick="sortTable(2)">Poster<i class="fa fa-sort"></i></th>
    <th onclick="sortTable(2)">Case<i class="fa fa-sort"></i></th>
  </tr>
  </thead>
  <tbody id = "myTable">
        <tr>
            <td>2011</td>
            <td>Asura: The City of Madness</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/e/e5/Asura_The_City_of_Madness_poster.jpeg" width="60%"></td>
            <td>大庄洞</td>
        </tr>
        <tr>
            <td>1997</td>
            <td>Default</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/5/55/Sovereign_Default.jpg" width="60%"></td>
            <td>IMF</td>
        </tr>
        <tr>
            <td>1987</td>
            <td>1987: When the Day Comes</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/8/87/1987_When_the_Day_Comes.jpg" width="60%"></td>
            <td>6·10民主抗爭</td>
        </tr>
        <tr>
            <td>1979</td>
            <td>The Man Standing Next</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/0/0b/The_Man_Standing_Next_movie_poster%2C_Jan_2020.jpg" width="60%"></td>
            <td>10.26</td>
        </tr>
        <tr>
            <td>1979</td>
            <td>The President's Last Bang</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/b/b6/President%27s_Last_Bang_Poster.jpg" width="60%"></td>
            <td>10.26</td>
        </tr>
        <tr>
            <td>1637</td>
            <td>The Fortress</td>
            <td><img src ="https://upload.wikimedia.org/wikipedia/en/0/0d/The_Fortress_-_%EB%82%A8%ED%95%9C%EC%82%B0%EC%84%B1.jpg" width="60%"></td></td>
            <td>丙子胡亂</td>
        </tr>
    </tbody>
  </table>

</body>
</html>
