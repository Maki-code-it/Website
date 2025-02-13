<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Will You Be My Valentine?</title>  
    <style>  
        body {  
            font-family: Arial, sans-serif;  
            text-align: center;  
            padding: 50px;  
            background-color: #D70040;  
        }  
        button {  
            margin: 10px;  
            padding: 10px 20px;  
            font-size: 16px;  
            border: none;  
            border-radius: 5px;  
            background-color: #ff69b4;  
            color: white;  
            cursor: pointer;  
        }  
        button:hover {  
            background-color: #ff1493;  
        }  
        #gifsContainer {  
            display: flex; /* Use flexbox for horizontal layout */  
            justify-content: center; /* Center horizontally */  
            flex-wrap: wrap; /* Allow wrapping if needed */  
        }  
        .gif {  
            display: none;  /* Hide the GIFs initially */  
            margin: 10px; /* Add some spacing around each GIF */  
        }  
    </style>  
</head>  
<body>  
    <h1>😈 IKAW VALENTINES KU? 😈</h1>  
    <p>PELE KA DETU:</p>  
    <button onclick="handleResponse('yes')">Yes</button>  
    <button onclick="handleResponse('no')">No</button>  

    <audio id="myAudio" src="anuto.mp3"></audio>  

    <div id="gifsContainer">  
        <img class="gif" src="200.webp"  width="300" />  
        <img class="gif" src="dog1.webp"  width="300" />  
        <img class="gif" src="cat1.webp"  width="300" />  
        <img class="gif" src="cat2.webp"  width="300" />  
    </div>  

    <script>  
        function handleResponse(response) {  
            const audio = document.getElementById('myAudio');  
            const gifs = document.querySelectorAll('.gif');  
            
            gifs.forEach(gif => gif.style.display = 'none');  

            if (response === 'yes') {  
                alert("Yay! I'm so glad! 🎊");  
                audio.play();  
                
                gifs.forEach(gif => gif.style.display = 'block'); 
            } else {  
                alert("ANONG NO BAWAL UN ANONG SINASABE MO EDI HINDI AKO??");  
            }  
        }  
    </script>  
</body>  
</html>
