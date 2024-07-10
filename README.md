<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Master Schedule 2023-2024</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>Master Schedule 2023-2024</h1>
        <div class="tabs">
            <button class="tablink" onclick="openTab(event, 'InspectTestCM')">Inspect, Test, CM</button>
            <button class="tablink" onclick="openTab(event, 'SCHCCO')">SCH CCO</button>
            <button class="tablink" onclick="openTab(event, 'RawDataSchedule')">Raw Data Schedule</button>
            <button class="tablink" onclick="openTab(event, 'PMTaskMaterialList')">PM Task Material List</button>
        </div>

        <div id="InspectTestCM" class="tabcontent">
            <!-- Table for Inspect, Test, CM will go here -->
        </div>
        <div id="SCHCCO" class="tabcontent">
            <!-- Table for SCH CCO will go here -->
        </div>
        <div id="RawDataSchedule" class="tabcontent">
            <!-- Table for Raw Data Schedule will go here -->
        </div>
        <div id="PMTaskMaterialList" class="tabcontent">
            <!-- Table for PM Task Material List will go here -->
        </div>
    </div>

    <script src="scripts.js"></script>
</body>
</html>
/* styles.css */
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    margin: 0;
    padding: 20px;
}

.container {
    background-color: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
}

h1 {
    text-align: center;
}

.tabs {
    display: flex;
    justify-content: center;
    margin-bottom: 20px;
}

.tablink {
    background-color: #555;
    color: white;
    padding: 14px 20px;
    margin: 0 5px;
    border: none;
    cursor: pointer;
    transition: background-color 0.3s;
}

.tablink:hover {
    background-color: #777;
}

.tabcontent {
    display: none;
    padding: 20px;
    border-top: 1px solid #ddd;
}

.active {
    display: block;
}

table {
    width: 100%;
    border-collapse: collapse;
}

table, th, td {
    border: 1px solid #ddd;
}

th, td {
    padding: 8px;
    text-align: left;
}

th {
    background-color: #f2f2f2;
}
/* scripts.js */
function openTab(evt, tabName) {
    var i, tabcontent, tablinks;
    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
        tabcontent[i].style.display = "none";
    }
    tablinks = document.getElementsByClassName("tablink");
    for (i = 0; i < tablinks.length; i++) {
        tablinks[i].className = tablinks[i].className.replace(" active", "");
    }
    document.getElementById(tabName).style.display = "block";
    evt.currentTarget.className += " active";
}
<!-- Table for Inspect, Test, CM -->
<div id="InspectTestCM" class="tabcontent">
    <table>
        <thead>
            <tr>
                <th>Location</th>
                <th>PYRITE PLANT</th>
                <th>&lt;--- Please select area</th>
                <!-- Add more headers as needed -->
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Type</td>
                <td>(All)</td>
                <td></td>
                <!-- Add more columns as needed -->
            </tr>
            <tr>
                <td>Status Required</td>
                <td>(Multiple Items)</td>
                <td>Do it when equipt runs or Down</td>
                <!-- Add more columns as needed -->
            </tr>
            <!-- Add more rows as needed -->
        </tbody>
    </table>
</div>
