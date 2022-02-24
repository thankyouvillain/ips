---
date: 2010-09-10 12:26:40
layout: post
title: Bookmark
subtitle: Lorem ipsum dolor sit amet, consectetur adipisicing elit.
description: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
image: https://res.cloudinary.com/dm7h7e8xj/image/upload/v1559825145/theme16_o0seet.jpg
optimized_image: https://res.cloudinary.com/dm7h7e8xj/image/upload/c_scale,w_380/v1559825145/theme16_o0seet.jpg
category: life
tags:
  - life
  - tips
author: thiagorossener
---

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
