---
date: 2010-09-10 12:26:40
layout: post
title: Birds can fly, but this you knew already
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

<html>
  <head>

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
          [ 'Koo Kyo-hwan', 'Peninsula',    new Date(2020,7,15,0,0,0),  new Date(2021,7,23,0,0,0) ],
          [ 'Koo Kyo-hwan', 'Kingdom: Ashin of the North',    new Date(2021,7,23,0,0,0),  new Date(2021,7,28,0,0,0) ],
          [ 'Koo Kyo-hwan', 'Escape from Mogadishu',    new Date(2021,7,28,0,0,0),  new Date(2021,8,27,0,0,0) ],
          [ 'Koo Kyo-hwan', 'D.P.',    new Date(2021,8,27,0,0,0),  new Date(2022,2,22,0,0,0) ],
          [ 'Yoo Ah-in', 'Default',    new Date(2018,11,28,0,0,0),  new Date(2021,6,24,0,0,0) ],
          [ 'Yoo Ah-in', '#Alive',    new Date(2021,6,24,0,0,0),  new Date(2021,10,15,0,0,0) ],
          [ 'Yoo Ah-in', 'Voice of Silence',    new Date(2021,10,15,0,0,0),  new Date(2021,11,19,0,0,0) ],
          [ 'Yoo Ah-in', 'Hellbound',    new Date(2021,11,19,0,0,0),  new Date(2022,2,22,0,0,0) ],
          ]);
    
        var options = {
          timeline: { colorByRowLabel: true }
        };
    
        chart.draw(dataTable, options);
      }
    
    </script>
    
    <div id="example5.1" style="height: 100%;"></div>
</html>









