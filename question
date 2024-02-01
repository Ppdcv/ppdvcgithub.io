<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Day Invitation</title>
    <style>
        body {
            text-align: center;
            margin: 0;
            padding: 0;
            overflow: hidden;
            background-color: #FFC0CB; /* Rose */
        }
        .heart {
            position: absolute;
            width: 10px;
            height: 10px;
            background-color: red;
            clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
            animation: heartAnimation 2s linear infinite;
        }
        #question {
            font-size: 24px;
            margin-top: 50px;
        }
        #choices {
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <h1>Invitation spéciale pour la Saint-Valentin</h1>
    <div id="question">Veux-tu être mon Valentine ?</div>
    <div id="choices">
        <button onclick="repondre(true)">Oui</button>
        <button onclick="repondre(false)">Non</button>
    </div>

    <script>
        function createHeart() {
            const heart = document.createElement('div');
            heart.className = 'heart';
            heart.style.left = Math.random() * window.innerWidth + 'px';
            document.body.appendChild(heart);

            setTimeout(() => {
                heart.remove();
            }, 2000);
        }

        function repondre(choix) {
            const questionDiv = document.getElementById('question');
            const choicesDiv = document.getElementById('choices');

            questionDiv.innerHTML = choix ? 'C\'est génial ! Joyeuse Saint-Valentin !' : 'Tant pis, tu le seras quand même.';
            choicesDiv.innerHTML = '';

            if (choix) {
                const grosCoeur = document.createElement('div');
                grosCoeur.innerHTML = '&#10084;&#10084;&#10084;';
                grosCoeur.style.fontSize = '48px';
                grosCoeur.style.color = 'red';
                document.body.appendChild(grosCoeur);
            }
        }

        function heartAnimation() {
            createHeart();
        }

        setInterval(heartAnimation, 500); // Crée un cœur toutes les 0.5 secondes
    </script>

</body>
</html>
