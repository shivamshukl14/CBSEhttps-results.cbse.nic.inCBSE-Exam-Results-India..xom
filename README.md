<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CBSE Result 2025</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
            color: #333;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #2c3e50;
            color: white;
            padding: 20px;
            text-align: center;
        }

        h1 {
            margin: 0;
            font-size: 24px;
        }

        .form-section {
            background-color: #ffffff;
            padding: 20px;
            margin: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        h2 {
            font-size: 20px;
        }

        label {
            display: block;
            margin-bottom: 8px;
            font-size: 14px;
        }

        input[type="text"] {
            width: 100%;
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 14px;
        }

        button {
            background-color: #3498db;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }

        button:hover {
            background-color: #2980b9;
        }

        .result-section {
            background-color: #ffffff;
            padding: 20px;
            margin: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }

        th, td {
            border: 1px solid #ddd;
            padding: 12px;
            text-align: center;
        }

        th {
            background-color: #f2f2f2;
        }

        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        footer p {
            margin: 0;
            font-size: 12px;
        }
    </style>
</head>
<body>
    <header>
        <h1>CBSE Result 2025 - Secondary School Examination</h1>
    </header>

    <section class="form-section">
        <h2>Enter Your Details</h2>
        <form id="resultForm">
            <label for="name">Student Name:</label>
            <input type="text" id="name" required>

            <label for="roll">Roll Number:</label>
            <input type="text" id="roll" required>

            <label for="dob">Date of Birth:</label>
            <input type="text" id="dob" required>

            <label for="school">School Name:</label>
            <input type="text" id="school" required>

            <button type="submit">View Result</button>
        </form>
    </section>

    <section id="resultSection" class="result-section" style="display:none;">
        <h2>Your CBSE Result</h2>
        <p id="resultName"></p>
        <p id="resultRoll"></p>
        <p id="resultDob"></p>
        <p id="resultSchool"></p>

        <table>
            <thead>
                <tr>
                    <th>Subject</th>
                    <th>Marks Obtained</th>
                    <th>Grade</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>English</td>
                    <td>85</td>
                    <td>A2</td>
                </tr>
                <tr>
                    <td>Mathematics</td>
                    <td>90</td>
                    <td>A1</td>
                </tr>
                <tr>
                    <td>Science</td>
                    <td>78</td>
                    <td>B1</td>
                </tr>
                <tr>
                    <td>Social Science</td>
                    <td>88</td>
                    <td>A2</td>
                </tr>
                <tr>
                    <td>Hindi</td>
                    <td>80</td>
                    <td>A2</td>
                </tr>
            </tbody>
        </table>

        <p id="resultSummary"></p>
    </section>

    <footer>
        <p>Disclaimer: This is a prank result sheet created for fun purposes only.</p>
    </footer>

    <script>
        document.getElementById('resultForm').addEventListener('submit', function(event) {
            event.preventDefault();

            var name = document.getElementById('name').value;
            var roll = document.getElementById('roll').value;
            var dob = document.getElementById('dob').value;
            var school = document.getElementById('school').value;

            // Display the result section
            document.getElementById('resultSection').style.display = 'block';

            // Populate the result information
            document.getElementById('resultName').textContent = 'Student Name: ' + name;
            document.getElementById('resultRoll').textContent = 'Roll Number: ' + roll;
            document.getElementById('resultDob').textContent = 'Date of Birth: ' + dob;
            document.getElementById('resultSchool').textContent = 'School: ' + school;

            // Calculate total marks and display division
            var totalMarks = 85 + 90 + 78 + 88 + 80;
            var division = totalMarks >= 400 ? 'First Division' : totalMarks >= 300 ? 'Second Division' : 'Third Division';
            document.getElementById('resultSummary').textContent = 'Total Marks: ' + totalMarks + ' / 500, ' + division;
        });
    </script>
</body>
</html>
