<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Number Guessing Game Flowchart</title>
    <script type="module">
      import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
      mermaid.initialize({ startOnLoad: true });
    </script>
</head>
<body>
    <div class="mermaid">
    graph TD
        A[Start] --> B[Initialize Game]
        B --> C[Generate Random Number]
        C --> D[Player Makes a Guess]
        D --> E{Is the Guess Correct?}
        E -->|Yes| F[Player Wins!]
        E -->|No| G{Is the Guess Too High?}
        G -->|Yes| H[Inform Player: "Too High"]
        G -->|No| I[Inform Player: "Too Low"]
        H --> J[Player Makes Another Guess]
        I --> J
        J --> D
        F --> K[End Game]
    </div>
</body>
</html>
