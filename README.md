<!DOCTYPE html>
<html>
<head>
    <title>My Simple Web Page</title>
    <style>
         /* Add a beautiful blue border at the top of the page */
         body {
            margin-top: 10px;
            border-top: 5px solid #31ff1e; /* Bright blue color */
            background: linear-gradient(to right, #1E90FF, #00BFFF); /* Blue gradient */
        }
        /* Style for images to make them responsive */
        .zoom-container {
            overflow: hidden;
            display: inline-block;
            max-width: 100%; /* Prevent overflow */
        }
        .zoom-container img {
            width: 100%;
            height: auto;
            transition: transform 0.25s ease;
            cursor: pointer; /* Make cursor pointer to show it's clickable */
        }

        /* Button style */
        .zoom-btns {
            margin: 20px 0;
        }
        .zoom-btns button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            margin: 5px;
        }

        /* Chatbot styling */
        .chatbot {
            position: fixed;
            bottom: 20px;
            right: 20px;
            width: 300px;
            height: 400px;
            border: 1px solid #ccc;
            background-color: #fff;
            padding: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .chatbox {
            width: 100%;
            height: 300px;
            overflow-y: auto;
            border-bottom: 1px solid #ccc;
            padding: 10px;
        }
        .chat-input {
            width: 100%;
            padding: 10px;
            margin-top: 10px;
        }

        /* Footer Border */
        footer {
            border-top: 5px solid black;  /* Black border at the top of the footer */
            text-align: center;
            padding: 20px;
            background-color: #47ce25;
        }
    </style>
</head>
<body>
    <header>
        <h1>..........Welcome H.B WEB world #>LANGAY>UN>13 LANGAY HIGH SCHOOL</h1>
        <H2>..........ITS NOT MY PROFASONAL PAGE BUT IF YOU ARE INTRASTED FOR  YOUR OWEN WEBSITE THEN CONTECT US ON THIS EMAIL</H2>
        <H1>..........HASEEBAH725@GMAIL.COM..............................................................................</H1>
        <H4>==========WE JUST HEAR TO HELP PEOPLE AND FOR BUILD A BETTER AND GOOD AND SUCCESFULL COMUNITY IN EDUCATION THROUGH MODRAN AI</H4>
    </header>
    <!-- First Image with zoom controls -->
    <div class="zoom-container" id="zoom1">
        <img id="image1" src="https://miro.medium.com/v2/resize:fit:720/format:webp/1*1hMun_WzCl02tpQePIV66Q.jpeg" alt="Personal Blog Image" width="1920" height="1080" onclick="toggleImageSize('image1')">
    </div>
    <div class="zoom-btns">
        <button onclick="zoomIn('image1')">Zoom In</button>
        <button onclick="zoomOut('image1')">Zoom Out</button>
    </div>
    <section>
        <h2>
        <P> OPEN CHART BORT IS AVILABAL ON OUR PAGE FEEL FREE AND ASKE ANY QUASTION</P>
        <P><H1> 👇 WARRAICH BRITHER GUJRAT LANGAY OUR WORK PROMOTING ONLINE BUSENISS AS WEBMASTER</H1></P>
        </h2>
    </section>
    <!-- Second Image with zoom controls -->
    <div class="zoom-container" id="zoom2">
        <img id="image2" src="https://miro.medium.com/v2/resize:fit:720/format:webp/1*gJWza27TjSQ2bnbpHeJGtQ.jpeg" alt="Second Image" width="1920" height="1080" onclick="toggleImageSize('image2')">
    </div>
    <div class="zoom-btns">
        <button onclick="zoomIn('image2')">Zoom In</button>
        <button onclick="zoomOut('image2')">Zoom Out</button>
    </div>
   <!-- Third Image with zoom controls -->
<div class="zoom-container" id="zoom3">
    <img id="image3" src="https://miro.medium.com/v2/resize:fit:720/format:webp/1*mjwjT4PcZyFYDnFwhb7U3w.jpeg" alt="Third Image" width="1920" height="1080" onclick="toggleImageSize('image3')">
</div>
<div class="zoom-btns">
    <button onclick="zoomIn('image3')">Zoom In</button>
    <button onclick="zoomOut('image3')">Zoom Out</button>
</div>
     <section>
        <h2>About Me</h2>
        <h>
        <P> YOU CAN ASKE ME ANQUASTION IT WILL DIRACTLY CONECT YOU WITH OPEN ai</P>
        <p>AND GET YOU ANSWEAR EASLY</p>
        <p>Hello! I AM HASEEB AKBAR ORF FUJI AKBAR WARRAICH GROUP LANGAY !</p>
        <p>IF YOU WANT TO REED ABOUT WARRAICH PERSONALITY GO THE LINK AND REED MORE THANK YOU</p>
        <p>REED ABOUT MY PERSONALITY👉 <a href="https://medium.com/@haseeb.akbar773/the-good-life-and-good-personality-a-journey-to-fulfillment-and-integrity-b33372929693">personal blog</a>.</p>
    </section>
        </h>
    <!-- Blog Link Added at the end -->
    <footer>
<p>The Good Life and Good Personality:allways posibal through educated socity (we) (us) (one)<a href="https://medium.com/@haseeb.akbar773/the-good-life-and-good-personality-a-journey-to-fulfillment-and-integrity-b33372929693"</a></p>
    </footer>

    <!-- Chatbot Section -->
    <div class="chatbot" id="chatbot">
        <div class="chatbox" id="chatbox">
            <div class="chat-message">Hello! I'm here to answer YOUR ALL QUASTIONS START TO WRITE AND GO TO THE PAGE👇<a href="https://chatgpt.com/". </div>
        <input type="text" id="userInput" class="chat-input" placeholder="Ask me anything..." onkeydown="if(event.key === 'Enter'){getAnswer()}">
    </div>

    <script>
        // Initial zoom level
        const zoomLevels = {
            "image1": 1,
            "image2": 1
        };

        // Function to zoom in
        function zoomIn(imageId) {
            const image = document.getElementById(imageId);
            zoomLevels[imageId] += 0.2; // Increase zoom level by 0.2
            image.style.transform = `scale(${zoomLevels[imageId]})`; // Apply zoom
        }

        // Function to zoom out
        function zoomOut(imageId) {
            const image = document.getElementById(imageId);
            if (zoomLevels[imageId] > 1) {
                zoomLevels[imageId] -= 0.2; // Decrease zoom level by 0.2 but not below 1
                image.style.transform = `scale(${zoomLevels[imageId]})`; // Apply zoom
            }
        }

        // Function to toggle image size (click to enlarge to 1920x1080 or back to original size)
        function toggleImageSize(imageId) {
            const image = document.getElementById(imageId);
            if (image.style.width !== '1920px') {
                image.style.width = '1920px'; // Set image width to 1920px
                image.style.height = '1080px'; // Set image height to 1080px
            } else {
                image.style.width = '100%'; // Revert back to responsive size
                image.style.height = 'auto'; // Revert height to auto
            }
        }

        // Function to handle chat interactions
        function getAnswer() {
            const userInput = document.getElementById("userInput").value.toLowerCase();
            const chatbox = document.getElementById("chatbox");

            // Predefined set of questions and answers
            let answer = "Sorry, I don't understand that question.";

            if (userInput.includes("hello")) {
                answer = "Hi there! How can I help you?";
            } else if (userInput.includes("your name")) {
                answer = "I'm your friendly chatbot!";
            } else if (userInput.includes("how are you")) {
                answer = "I'm just a program, but I'm doing great!";
            } else if (userInput.includes("your purpose")) {
                answer = "I'm here to assist you with your questions.";
            }

            // Display user question and bot answer
            const newMessage = document.createElement("div");
            newMessage.classList.add("chat-message");
            newMessage.textContent = "You: " + userInput;
            chatbox.appendChild(newMessage);

            const botMessage = document.createElement("div");
            botMessage.classList.add("chat-message");
            botMessage.textContent = "Bot: " + answer;
            chatbox.appendChild(botMessage);

            // Clear input field
            document.getElementById("userInput").value = "";

            // Scroll to the bottom of the chatbox
            chatbox.scrollTop = chatbox.scrollHeight;
        }
    </script>
</body>
</html>
