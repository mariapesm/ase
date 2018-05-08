  .pie { height: 500px; } body { font-family: constantia; background-color: #fffff; } a, a:visited { color: white } hr { height: 5px; border: 0; background: black; }

Disposal time of garbage
========================

[](https://code.google.com/apis/ajax/playground/)  |  [](https://developers.google.com/chart/interactive/docs/customizing_charts)

google.load("visualization", "1", {packages:\["corechart"\]}); google.setOnLoadCallback(drawChart); function drawChart() { var data = google.visualization.arrayToDataTable(\[ \['Materials', 'Age', 'Object Disintegration Time', \], \['Paper', 2, 'Weeks'\], \['Orange', 5, 'Weeks'\], \['Plant leaves', 3, 'Months'\], \['Cotton fabric', 5, 'Months'\], \['Rope', 14, 'Months'\], \['Bamboo stick', 3, 'Years'\], \['Woolen cloth', 1, 'Years'\], \['Suture', 5, 'Years'\], \['Plastic coated paper', 5, 'Years'\], \['Plastic bag', 10, 'Years'\], \['Baby nap', 20, 'Years'\], \['Plastic glass', 250, 'Years'\], \['Plastic bottle', 450, 'Years'\], \['Materials from nylon', 40, 'Years'\], \['Aluminum cans', 500, 'Years'\], \['Canned Tuna', 100, 'Years'\], \['Glass unknown', 500,'Years'\], \]); var chart = new google.visualization.PieChart(document.getElementById('pie')); chart.draw(data, { //title: '2D pie chart', is3D: '', legend: 'yes', backgroundColor: 'transparent', pieSliceBorderColor: 'transparent', pieSliceText: 'yes', colors: \['#f7ec00', '#00aaad', '#fff71a', '#ffa226', '#4064dd'\], chartArea:{left:"25%",top:10,width:"400%"}, tooltip: {textStyle: {color: 'black'}, showColorCode: true} }); } //# sourceURL=pen.js
