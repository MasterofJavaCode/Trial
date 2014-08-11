Trial
=====
=====
<DOCTYPE html>
<head>
  <script type="text/javascript" src="https://www.google.com/jsapi"></script>
    <script type="text/javascript">
      google.load("visualization", "1", {packages:["corechart"]});
      google.setOnLoadCallback(drawChart);
      function drawChart() {
        var data = google.visualization.arrayToDataTable([
          ['Opinion', 'Percentage Teachers'],
          ['Approve',     75],
          ['Disapprove',      22],
          ['No Opnion',  3],
        
        ]);

        var options = {
          title: 'Teachers Opinions of Common Core'
        };

        var chart = new google.visualization.PieChart(document.getElementById('piechart'));
        chart.draw(data, options);
      }
    </script>
</head>
  <body>
    <div id="piechart" style="width: 900px; height: 500px;"></div>
  </body>

</html>

