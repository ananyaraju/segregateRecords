# segregateRecords
Consider a sample csv [<a href="https://github.com/ananyaraju/segregateRecords/blob/main/demo.csv">demo.csv</a>] containing names and a corresponding array of types it belongs to.
Having an array as a field entry becomes problematic for visualization of such a csv.
This is because a field entry [CompanyX, "Retail, Wholesale"] will create a logically new "type" and showcase this array as a whole different category, instead of counting CompanyX under BOTH Retail and Wholesale type of businesses.
The pie chart visualization of <a href="https://github.com/ananyaraju/segregateRecords/blob/main/demo.csv">demo.csv</a> is given below:
<div align="center">
  <img src="https://github.com/ananyaraju/segregateRecords/blob/main/visualisations/incorrectVisualization.png" height="350" />
</div>
<br>
Clearly, this visualization leads to improper and inaccurate data representation.
<br><br>
The correct way to visualize this would be to seperate every element in the "Type" array as a different entry in csv, leading to explosion of data within the csv.
After running the <a href="https://github.com/ananyaraju/segregateRecords/blob/main/segregateType.ipynb">segregateType.ipynb</a> program and generating a new csv [<a href="https://github.com/ananyaraju/segregateRecords/blob/main/final.csv">final.csv</a>] with exploded data, the pie chart visualization of the csv is as follows:
<div align="center">
  <img src="https://github.com/ananyaraju/segregateRecords/blob/main/visualisations/correctVisualization.png" height="350" />
</div>
