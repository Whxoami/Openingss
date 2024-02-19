<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chess Openings</title>
</head>
<body>
    <h1>Chess Openings Explained</h1>
    <button onclick="showOpening('italian')">Italian Game</button>
    <button onclick="showOpening('sicilian')">Sicilian Defense</button>
    <button onclick="showOpening('french')">French Defense</button>
    <button onclick="showOpening('caro-kann')">Caro-Kann Defense</button>
    <button onclick="showOpening('ruy-lopez')">Ruy Lopez</button>

    <div id="opening-description">
        <!-- Opening descriptions will be displayed here -->
    </div>

    <script>
        function showOpening(opening) {
            var description = "";

            switch (opening) {
                case "italian":
                    description = "The Italian Game is a popular opening that begins with the moves 1.e4 e5 2.Nf3 Nc6 3.Bc4. It aims to control the center and develop pieces quickly.";
                    break;
                case "sicilian":
                    description = "The Sicilian Defense is a sharp and dynamic response to 1.e4. Black plays 1...c5, aiming for counterplay on the d4-square and often leading to complex positions.";
                    break;
                case "french":
                    description = "The French Defense begins with 1.e4 e6, aiming to control the center with pawns and later strike at the center with moves like ...d5. It leads to solid and strategic positions for Black.";
                    break;
                case "caro-kann":
                    description = "The Caro-Kann Defense is a solid and reliable opening for Black. It begins with 1.e4 c6, aiming for a strong pawn structure and solid development.";
                    break;
                case "ruy-lopez":
                    description = "The Ruy Lopez is one of the oldest and most respected openings in chess. It starts with 1.e4 e5 2.Nf3 Nc6 3.Bb5, leading to rich and nuanced positions.";
                    break;
                default:
                    description = "Select an opening to learn more about it.";
            }

            document.getElementById("opening-description").innerHTML = description;
        }
    </script>
</body>
</html>
