<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>site do kimura</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        a {
            text-decoration: none;
            /* Corrigido */
        }

        .box {
            font: 20px;
            color: aliceblue;
            height: 250px;
            /* Adicionada unidade de medida */
            width: 450px;
            /* Adicionada unidade de medida */
            border: 10px;
            background: #191919;
            flex-direction: column;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .buttons-container {
            display: flex;
            justify-content: space-around;
            height: 50px;
            width: 150px;
        }

        button {
            height: 30px;
            width: 50px;
            background: white;
            border-radius: 5px;
            color: blue;
        }
    </style>
</head>

<body>
    <div class="box">
        <p> mostra as tetas?</p>
        <div class="buttons-container">
            <button>
                <a href="">não</a>
            </button>
            <button id="no">sim</button>
        </div>
    </div>

    <script type="module">
        // Import the functions you need from the SDKs you need
        import { initializeApp } from "https://www.gstatic.com/firebasejs/10.11.1/firebase-app.js";
        import { getAnalytics } from "https://www.gstatic.com/firebasejs/10.11.1/firebase-analytics.js";
        // TODO: Add SDKs for Firebase products that you want to use
        // https://firebase.google.com/docs/web/setup#available-libraries

        // Your web app's Firebase configuration
        // For Firebase JS SDK v7.20.0 and later, measurementId is optional
        const firebaseConfig = {
            apiKey: "AIzaSyDPW9-4IL_vIHU2ajb09JGWlUpvKoj6PO4",
            authDomain: "malu-f5d69.firebaseapp.com",
            projectId: "malu-f5d69",
            storageBucket: "malu-f5d69.appspot.com",
            messagingSenderId: "128914455897",
            appId: "1:128914455897:web:2859ec260a20287033a048",
            measurementId: "G-6S8CTH0G3P"
        };

        // Initialize Firebase
        const app = initializeApp(firebaseConfig);
        const analytics = getAnalytics(app);
    </script>

    <script>
        let button = document.getElementById('no');
        let height = window.innerHeight - 50;
        let width = window.innerWidth - 50;

        button.addEventListener('mouseover', function () {
            button.style.position = "absolute";
            button.style.top = Math.random() * height + "px"; // Adicionada unidade de medida
            button.style.left = Math.random() * width + "px"; // Adicionada unidade de medida
        });
    </script>

</html>
