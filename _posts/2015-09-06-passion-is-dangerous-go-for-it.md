---
date: 2015-09-06 12:00:00
layout: post
title: Thankschool728
subtitle: Thankschool728's Space
description: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
image: https://upload.wikimedia.org/wikipedia/en/1/10/The_Greatest_Showman_poster.png
optimized_image: https://upload.wikimedia.org/wikipedia/en/1/10/The_Greatest_Showman_poster.png
category: work
tags:
  - work
  - career
author: thiagorossener
---
<html>

    <script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>

    <script type="text/javascript">
      google.charts.load("current", {packages:["timeline"]});
      google.charts.setOnLoadCallback(drawChart);
      function drawChart() {
    
        var container = document.getElementById('example5.1');
        var chart = new google.visualization.Timeline(container);
        var dataTable = new google.visualization.DataTable();
        dataTable.addColumn({ type: 'string', id: 'Room' });
        dataTable.addColumn({ type: 'string', id: 'Name' });
        dataTable.addColumn({ type: 'date', id: 'Start' });
        dataTable.addColumn({ type: 'date', id: 'End' });
        dataTable.addRows([
          [ 'HTML_Ban', 'Part1',       new Date(0,0,0,0,0,0),  new Date(0,0,0,0,1,9) ],
          [ 'HTML_Ban', 'Part_End',    new Date(0,0,0,0,7,17),  new Date(0,0,0,0,7,18) ],
          [ 'Design_Koba', 'Part1',       new Date(0,0,0,0,0,0),  new Date(0,0,0,0,0,25) ],
          [ 'Design_Koba', 'Part2',       new Date(0,0,0,0,4,44),  new Date(0,0,0,0,4,53) ],
          [ 'Design_Koba', 'Part_End',    new Date(0,0,0,0,5,43),  new Date(0,0,0,0,5,48) ],
          ]);
    
        var options = {
          timeline: { colorByRowLabel: true }
        };
    
        chart.draw(dataTable, options);
      }
    
    </script>
    <script type="text/javascript">
        google.charts.load("current", {packages:["timeline"]});
        google.charts.setOnLoadCallback(drawChart);
        function drawChart() {
      
          var container = document.getElementById('example4.1');
          var chart = new google.visualization.Timeline(container);
          var dataTable = new google.visualization.DataTable();
          dataTable.addColumn({ type: 'string', id: 'Room' });
          dataTable.addColumn({ type: 'string', id: 'Name' });
          dataTable.addColumn({ type: 'date', id: 'Start' });
          dataTable.addColumn({ type: 'date', id: 'End' });
          dataTable.addRows([
            [ 'Koo Kyo-hwan', 'Peninsula',    new Date(2020,7,15,0,0,0),  new Date(2021,7,23,0,0,0) ],
            [ 'Koo Kyo-hwan', 'Kingdom: Ashin of the North',    new Date(2021,7,23,0,0,0),  new Date(2021,7,28,0,0,0) ],
            [ 'Koo Kyo-hwan', 'Escape from Mogadishu',    new Date(2021,7,28,0,0,0),  new Date(2021,8,27,0,0,0) ],
            [ 'Koo Kyo-hwan', 'D.P.',    new Date(2021,8,27,0,0,0),  new Date(2022,2,22,0,0,0) ],
            [ 'Yoo Ah-in', 'Default',    new Date(2018,11,28,0,0,0),  new Date(2021,6,24,0,0,0) ],
            [ 'Yoo Ah-in', '#Alive',    new Date(2021,6,24,0,0,0),  new Date(2021,10,15,0,0,0) ],
            [ 'Yoo Ah-in', 'Voice of Silence',    new Date(2021,10,15,0,0,0),  new Date(2021,11,19,0,0,0) ],
            [ 'Yoo Ah-in', 'Hellbound',    new Date(2021,11,19,0,0,0),  new Date(2022,2,22,0,0,0) ],
            [ 'Oppadu', 'Part_1',    new Date(2020,3,18,0,0,0),  new Date(2020,4,1,0,0,0) ],
            [ 'Oppadu', 'Part_2',    new Date(2020,6,24,0,0,0),  new Date(2020,6,29,0,0,0) ],
            [ 'Oppadu', 'Part_Now',    new Date(2022,2,17,0,0,0),  new Date(2022,2,18,0,0,0) ]
            ]);
      
          var options = {
            timeline: { colorByRowLabel: true }
          };
      
          chart.draw(dataTable, options);
        }
      
      </script>
    
    <div id="example4.1" ></div>
    <div id="example5.1" ></div>
  
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
  
img {
  border-radius: 99%;
}
</style>
</head>
<body>

<p>Sports</p>
<input id="myInput" type="text" placeholder="Search">
<br><br>

<table>
  <thead>
  <tr>
    <th onclick="sortTable(0)">* <i class="fa fa-sort"></i></th> 
    <th onclick="sortTable(1)">Image <i class="fa fa-sort"></i></th> 
    <th onclick="sortTable(2)">Exercise<br><i class="fa fa-sort"></i></th>
    <th onclick="sortTable(3)">Special<i class="fa fa-sort"></i></th>
  </tr>
  </thead>
  <tbody id = "myTable">
       
        <tr>
            <td>NFL</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/thumb/a/a2/National_Football_League_logo.svg/800px-National_Football_League_logo.svg.png" width="30%"></td>
            <td>131</td>
            <td></td>
            </tr>
        <tr>
            <td>T1</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/thumb/f/f9/T1_logo.svg/1920px-T1_logo.svg.png" width="30%"></td>
            <td>91</td>
            <td></td>
        </tr>
        <tr>
            <td>Incheon United</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/thumb/6/66/Emblem_of_Incheon_United.svg/800px-Emblem_of_Incheon_United.svg.png" width="30%"></td>
            <td>58</td>
            <td></td>
        </tr>
        <tr>
            <td>Faker</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/commons/e/e6/Faker_at_the_2015.10.02_S5_Paris_day2.jpeg" width="30%"></td>
            <td>42</td>
            <td></td>
        </tr>
        <tr>
            <td>Worlds</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/thumb/5/5f/LOL_Worlds_logo.svg/1024px-LOL_Worlds_logo.svg.png" width="30%"></td>
            <td>31</td>
            <td></td>
        </tr>
        <tr>
            <td>Cincinnati Bengals</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/commons/thumb/8/81/Cincinnati_Bengals_logo.svg/1280px-Cincinnati_Bengals_logo.svg.png" width="30%"></td>
            <td>30</td>
            <td></td>
        </tr>
        <tr>
            <td>NBA playoffs</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/thumb/4/44/NBA_Playoffs_logo_%282018%29.svg/1920px-NBA_Playoffs_logo_%282018%29.svg.png" width="30%"></td>
            <td>28</td>
            <td>Play Offs</td>
        </tr>
        <tr>
            <td>South Korea national football</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/f/f8/South_Korea_national_football_team.png" width="30%"></td>
            <td>21</td>
            <td></td>
        </tr>
        <tr>
            <td>Francis Ngannou</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/commons/e/ea/Francis_Ngannou_photo.jpg" width="30%"></td>
            <td>17</td>
            <td></td>
        </tr>
        <tr>
            <td>North London derby</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/commons/thumb/8/8b/Spurs_vs_Arsenal%2C_Avril_2007.jpg/375px-Spurs_vs_Arsenal%2C_Avril_2007.jpg" width="30%"></td>
            <td>15</td>
            <td>Derby</td>
        </tr>
            <tr>
            <td>ASL</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/b/b0/Afreeca_ASL_logo.jpg" width="30%"></td>
            <td>12</td>
            <td></td>
        </tr>
        <tr>
            <td>Jaedong</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/commons/8/86/Hwaseung_Jaedong.JPG" width="30%"></td>
            <td>7</td>
            <td></td>
        </tr>

         <tr>
            <td>Jeonbuk Hyundai Motors</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/thumb/2/23/Jeonbuk_Hyundai_Motors.svg/1024px-Jeonbuk_Hyundai_Motors.svg.png" width="30%"></td>
            <td>6</td>
            <td>Anti</td>
        </tr>


    </tbody>
  </table>

</body>
</html>
  
