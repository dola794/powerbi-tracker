<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Welcome to the Dashboard</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        h1 {
            margin: 20px 0;
        }
        .container {
            max-width: 1200px;
            margin: auto;
            padding: 20px;
            background: white;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
        }
        .button {
            padding: 10px 20px;
            font-size: 16px;
            margin-top: 20px;
            cursor: pointer;
            border: none;
            background-color: #4CAF50;
            color: white;
            border-radius: 5px;
        }
        .button:hover {
            background-color: #45a049;
        }
        .link-container {
            display: none;
            margin-top: 30px;
        }
        .report-link {
            font-size: 18px;
            color: #007bff;
            text-decoration: none;
            font-weight: bold;
        }
        .report-link:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Welcome to the Dashboard</h1>
        <p>Click the button below to get the link to the report.</p>
        <button class="button" onclick="showLink()">Show Report Link</button>

        <!-- Hidden container with the link -->
        <div class="link-container" id="linkContainer">
            <h2>Here is the link to the Power BI report:</h2>
            <a class="report-link" 
                href="https://app.powerbi.com/view?r=eyJrIjoiOWFlNzEzNGYtNWIxNC00ZTAyLThjYTgtNWZkMWUwNTRiZTk3IiwidCI6ImM3YmNkYzYzLTI4M2MtNDk5OC05NTk0LTQ1NTM5MzNlNGQ1YiIsImMiOjl9" 
                target="_blank">
                View the Power BI Report
            </a>
        </div>
    </div>

    <script>
        function showLink() {
            // Hide the button and show the link container
            document.querySelector('button').style.display = 'none';
            document.getElementById('linkContainer').style.display = 'block';
        }
    </script>
</body>
</html>
