<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rubriques</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            text-align: center;
        }

        h1 {
            cursor: pointer;
            color: #007bff;
            margin-top: 50px;
            text-decoration: underline;
        }

        .chevre-img {
            display: none;
            margin-top: 20px;
        }

        .show {
            display: block;
        }
    </style>
</head>
<body>
    <h1 onclick="toggleImage('lionel')">Lionel le brel</h1>
    <img id="lionel-img" class="chevre-img" src="lien_vers_votre_image_lionel.jpg" alt="Lionel le brel">
    <h1 onclick="toggleImage('maman')">Maman la chiante</h1>
    <img id="maman-img" class="chevre-img" src="lien_vers_votre_image_maman.jpg" alt="Maman la chiante">

    <script>
        function toggleImage(name) {
            const image = document.getElementById(name + "-img");
            image.classList.toggle("show");
        }
    </script>
</body>
</html>
