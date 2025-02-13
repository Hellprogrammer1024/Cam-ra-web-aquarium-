# Contenu HTML
html_content = """
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flux Vidéo en Direct de l'Aquarium</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
        }
        video {
            border: 5px solid #007BFF;
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <video id="aquariumVideo" width="640" height="480" controls autoplay>
        <source src="URL_DU_FLUX_VIDÉO" type="video/mp4">
        Votre navigateur ne supporte pas la balise vidéo.
    </video>

    <script>
        // Vous pouvez ajouter du JavaScript ici si nécessaire
    </script>
</body>
</html>
"""

# Écrire le contenu dans un fichier HTML
with open("aquarium_live.html", "w", encoding="utf-8") as file:
    file.write(html_content)

print("Le fichier HTML a été créé avec succès.")
