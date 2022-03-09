---
date: 2017-06-08 12:00:00
layout: post
title: Do you believe that a spider can dance?
subtitle: Lorem ipsum dolor sit amet, consectetur adipisicing elit.
description: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
category: travel
image: https://res.cloudinary.com/dm7h7e8xj/image/upload/v1559824306/theme13_dshbqx.jpg
optimized_image: https://res.cloudinary.com/dm7h7e8xj/image/upload/c_scale,w_380/v1559824306/theme13_dshbqx.jpg
tags:
  - fate
  - travel
author: thiagorossener
---

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
    <th onclick="sortTable(2)">Language<br><i class="fa fa-sort"></i></th>
    <th onclick="sortTable(3)">Hour<i class="fa fa-sort"></i></th>
  </tr>
  </thead>
  <tbody id = "myTable">
       
        <tr>
            <td>Dune</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/8/8e/Dune_%282021_film%29.jpg" width="30%"></td>
            <td>English</td>
            <td>2.60</td>
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
