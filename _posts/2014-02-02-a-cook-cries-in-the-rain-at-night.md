---
date: 2017-06-04 12:00:00
layout: post
title: A cook cries in the rain at night
subtitle: Lorem ipsum dolor sit amet, consectetur adipisicing elit.
description: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
image: https://res.cloudinary.com/dm7h7e8xj/image/upload/v1559824575/theme14_gi2ypv.jpg
optimized_image: https://res.cloudinary.com/dm7h7e8xj/image/upload/c_scale,w_380/v1559824575/theme14_gi2ypv.jpg
category: diet
tags:
  - cook
  - cucine
  - story
author: thiagorossener
---

 <!DOCTYPE html>
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

<p>English Subtitle_Book</p>
<input id="myInput" type="text" placeholder="Search">
<br><br>

<table>
  <thead>
  <tr>
    <th onclick="sortTable(0)">Title <i class="fa fa-sort"></i></th> 
    <th onclick="sortTable(1)">Language<i class="fa fa-sort"></i></th> 
    <th onclick="sortTable(2)">Poster<i class="fa fa-sort"></i></th>
    <th onclick="sortTable(3)">my<br>rating<i class="fa fa-sort"></i></th>
    <th onclick="sortTable(3)">#<i class="fa fa-sort"></i></th>
  </tr>
  </thead>
  <tbody id = "myTable">
        <tr>
            <td>Inception:<br>The Shooting Scrip</td>
            <td>English</td>
            <td><img src="https://images-na.ssl-images-amazon.com/images/I/61cOm8-xzTL._SX328_BO1,204,203,200_.jpg" width = "100%"></td>
            <td>10</td>
            <td>#Mind</td>
        </tr>
        <tr>
            <td>Inside<br>Out</td>
            <td>English</td>
            <td><img src="https://upload.wikimedia.org/wikipedia/en/0/0a/Inside_Out_%282015_film%29_poster.jpg" width = "100%"></td>
            <td>10</td>
            <td>#Mind</td>
        </tr>
        <tr>
            <td>Digital<br>Fortress</td>
            <td>English</td>
            <td><img src ="https://i.gr-assets.com/images/S/compressed.photo.goodreads.com/books/1360095966l/11125.jpg" width = "100%"></td>
            <td>10</td>
            <td>#Dan Brown</td>
        </tr>
        <tr>
            <td>Deception<br>Point</td>
            <td>English</td>
            <td><img src ="https://images-eu.ssl-images-amazon.com/images/I/41T7ZrFJefL._SY264_BO1,204,203,200_QL40_FMwebp_.jpg" width = "100%"></td>
            <td>10</td>
            <td>#Dan Brown</td>
        </tr>
        <tr>
            <td>Angels&<br>Demons</td>
            <td>English</td>
            <td><img src ="https://images-na.ssl-images-amazon.com/images/I/510uIcLWISL._SX327_BO1,204,203,200_.jpg" width = "100%"></td>
            <td>10</td>
            <td>#Dan Brown</td>
        </tr>
        <tr>
            <td>Extracurricular</td>
            <td>Korean</td>
            <td><img src="https://upload.wikimedia.org/wikipedia/en/9/9a/Extracurricular_2020.jpg" width="100%"></td>
            <td>9</td>
            <td>#School</td>
        </tr>
        <tr>
            <td>Money</td>
            <td>Korean</td>
            <td><img src="https://upload.wikimedia.org/wikipedia/en/f/f7/Money_%282019_film%29.jpg" width="100%"></td>
            <td>6</td>
            <td>#Economy<br>#Office</td>
        </tr>
        <tr>
            <td>Misaeng:<br>Incomplete<br>Life </td>
            <td>Korean</td>
            <td><img src="https://upload.wikimedia.org/wikipedia/en/e/e8/Misaeng-poster.jpg" width="100%"></td>
            <td>10</td>
            <td>#Office</td>
        </tr>
        <tr>
            <td>Stove<br>League</td>
            <td>Korean</td>
            <td><img src="https://upload.wikimedia.org/wikipedia/en/c/c9/Stove_League_main_poster.jpg" width="100%"></td>
            <td>10</td>
            <td>#School</td>
        </tr>
        <tr>
            <td>Master<br>of<br>Study</td>
            <td>Korean</td>
            <td><img src="https://upload.wikimedia.org/wikipedia/en/d/d3/LordofStudy.jpg" width="100%"></td>
            <td>10</td>
            <td>#Office<br>#Baseball</td>
        </tr>
        <tr>
            <td>Glove</td>
            <td>Korean</td>
            <td><img src="https://upload.wikimedia.org/wikipedia/en/2/2d/Glove2011Poster.jpg" width="100%"></td>
            <td>7</td>
            <td>#School<br>#Disabled<br>#Baseball</td>
        </tr>
        <tr>
            <td>All of us Are Dead</td>
            <td>Office</td>
            <td><img src="https://upload.wikimedia.org/wikipedia/en/2/24/All_of_Us_Are_Dead.jpeg" width="100%"></td>
            <td>5</td>
            <td>#School</td>
        </tr>
        <tr>
            <td>Songgot: The Piercery</td>
            <td>Office</td>
            <td>9</td>
            <td></td>
        </tr>
        <tr>
            <td>Solomon's Perjury</td>
            <td>School</td>
            <td>10</td>
            <td></td>
        </tr>
        <tr>
            <td>Along with the Gods: The Two Worlds</td>
            <td>沈pearl風</td>
            <td>7</td>
            <td>Original</td>
        </tr>
        <tr>
            <td>Along with the Gods: The Last 49 Days</td>
            <td>沈pearl風</td>
            <td>6</td>
            <td>Original</td>
        </tr>
        <tr>
            <td>Squid Game</td>
            <td>沈pearl風</td>
            <td>6</td>
            <td>Review</td>
        </tr>
        <tr>
            <td>Parasite</td>
            <td>沈pearl風</td>
            <td>7</td>
            <td>Review</td>
        </tr>
        <tr>
            <td>Hellbound</td>
            <td>沈pearl風</td>
            <td>9</td>
            <td>Review</td>
        </tr>
        <tr>
            <td>A Hard Day</td>
            <td>沈pearl風</td>
            <td>5</td>
            <td>Review</td>
        </tr>
    </tbody>
  </table>

</body>
</html>
