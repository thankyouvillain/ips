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
  padding: 10px;
  border-radius: 25px;
}
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
    <th onclick="sortTable(3)">Page<i class="fa fa-sort"></i></th>
  </tr>
  </thead>
  <tbody id = "myTable">
       
        <tr>
            <td>Dune</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/8/8e/Dune_%282021_film%29.jpg" width="60%"></td>
            <td>English</td>
            <td>2.60</td>
            <td></td>
            </tr>
        <tr>
            <td>Guardians of the Galaxy</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/3/33/Guardians_of_the_Galaxy_%28film%29_poster.jpg" width="60%"></td>
            <td>English</td>
            <td>2.03</td>
            <td></td>
        </tr>
         <tr>
            <td>Guardians of the Galaxy Vol. 2</td>
            <td><img src = "https://upload.wikimedia.org/wikipedia/en/a/ab/Guardians_of_the_Galaxy_Vol_2_poster.jpg" width="60%"></td>
            <td>English</td>
            <td>2.28</td>
            <td></td>
        </tr>   
        <tr>
            <td>Sum</td>
            <td></td>
            <td></td>
            <td>4.63</td>
            <td></td>
        </tr>
    </tbody>
  </table>

</body>
</html>
