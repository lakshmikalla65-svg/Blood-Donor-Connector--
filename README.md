### Blood Donor Connector

## Aim
To create a real-time system that connects hospitals with nearby voluntary blood donors during emergency situations.

## Description
Blood Donor Connector helps hospitals quickly find available blood donors based on blood group and location, reducing delay in critical situations.

## Features
- Donor registration
- Hospital request for blood
- Real-time donor notification
- Search by blood group and location

## Technologies Used
- Frontend: HTML, CSS, JavaScript
- Backend: Node.js / Python
- Database: MySQL / MongoDB

## Future Scope
- Mobile application
- GPS-based donor tracking
- SMS/WhatsApp alerts
## Code : -
<!DOCTYPE html>
<html>
<head>
    <title>Blood Donor Connector</title>
    <style>
        body {
            font-family: Arial;
            background-color: #f2f2f2;
            padding: 20px;
        }
        h1 {
            color: red;
        }
        button {
            padding: 8px 15px;
            background-color: red;
            color: white;
            border: none;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <h1>Blood Donor Connector</h1>
    <p>A real-time system connecting hospitals with voluntary blood donors.</p>

    <h2>Donor Registration</h2>
    <label>Name:</label><br>
    <input type="text" id="name"><br><br>

    <label>Blood Group:</label><br>
    <input type="text" id="blood"><br><br>

    <label>Location:</label><br>
    <input type="text" id="location"><br><br>

    <button onclick="registerDonor()">Register</button>

    <h3 id="output"></h3>

    <script>
        // Backend logic (simulated using JavaScript)
        function registerDonor() {
            var name = document.getElementById("name").value;
            var blood = document.getElementById("blood").value;
            var location = document.getElementById("location").value;

            if (name === "" || blood === "" || location === "") {
                document.getElementById("output").innerHTML =
                    "Please fill all details.";
            } else {
                document.getElementById("output").innerHTML =
                    "Donor " + name + " registered successfully!";
            }
        }
    </script>

</body>
</html>
