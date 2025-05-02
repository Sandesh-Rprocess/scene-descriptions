<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Scene Description</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .container {
            display: flex;
            justify-content: center;
            padding: 20px;
        }
        .video-container {
            width: 60%;
        }
        .description-container {
            width: 35%;
            margin-left: 20px;
        }
        .description-box {
            background-color: #fff;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        video {
            width: 100%;
            border-radius: 8px;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="video-container">
            <video id="videoPlayer" controls>
                <source src="your-video.mp4" type="video/mp4">
                Your browser does not support the video tag.
            </video>
        </div>
        <div class="description-container">
            <div class="description-box" id="foregroundDesc">Foreground: </div>
            <div class="description-box" id="backgroundDesc">Background: </div>
            <div class="description-box" id="subjectSubjectDesc">Subject-to-Subject: </div>
            <div class="description-box" id="subjectObjectDesc">Subject-to-Object: </div>
            <div class="description-box" id="objectObjectDesc">Object-to-Object: </div>
        </div>
    </div>

    <script>
        // Example of dynamically updating the descriptions based on video content
        const videoElement = document.getElementById('videoPlayer');

        // Simulating a function that updates descriptions
        function updateDescriptions() {
            // In practice, this would involve more complex logic with AI/ML
            document.getElementById('foregroundDesc').innerText = 'Foreground: Person walking.';
            document.getElementById('backgroundDesc').innerText = 'Background: Urban street, cars passing.';
            document.getElementById('subjectSubjectDesc').innerText = 'Subject-to-Subject: The person walks towards another.';
            document.getElementById('subjectObjectDesc').innerText = 'Subject-to-Object: The person touches a car.';
            document.getElementById('objectObjectDesc').innerText = 'Object-to-Object: Car and person interact.';
        }

        // Update descriptions every 2 seconds as an example (replace with real AI processing)
        setInterval(updateDescriptions, 2000);
    </script>

</body>
</html>
