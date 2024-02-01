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
            margin: 50px;
            font-family: 'Arial', sans-serif;
        }
        #hearts {
            display: none;
            font-size: 48px;
            color: red;
        }
    </style>
</head>
<body>

    <h1>Invitation spéciale pour la Saint-Valentin</h1>
    <a href="javascript:void(0);" onclick="showHearts()">Clique ici</a>

    <div id="hearts">&#10084;&#10084;&#10084;</div>

    <script>
        function showHearts() {
            document.getElementById('hearts').style.display = 'block';
            setTimeout(function() {
                var response = confirm("Veux-tu être mon Valentine ?");
                if (response) {
                    alert("C'est génial ! Joyeuse Saint-Valentin !");
                } else {
                    alert("Peut-être une autre fois. Bonne journée !");
                }
            }, 2000); // Les cœurs restent visibles pendant 2 secondes avant d'afficher la boîte de dialogue
        }
    </script>

</body>
</html>
