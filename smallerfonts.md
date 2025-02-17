<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Music Notation Shuffle</title>
    <style>
        body { 
            font-family: Arial, sans-serif; 
            text-align: center; 
            margin: 20px; 
        }

        h2 {
            font-size: 24px;
        }

        .note-buttons { 
            display: flex;
            justify-content: center;
            gap: 10px;
            margin: 20px; 
        }

        .column {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin: 0 10px;
        }

        button { 
            margin: 5px; 
            padding: 10px 15px; 
            font-size: 16px;
            border: none;
            background-color: #007BFF;
            color: white;
            border-radius: 5px;
            cursor: pointer;
            transition: 0.3s;
        }

        button:hover {
            background-color: #0056b3;
        }

        .message {
            font-size: 18px;
            margin-top: 20px;
            font-weight: bold;
            display: none;
        }

        /* Responsive Design */
        @media (max-width: 1024px) {
            h2 { font-size: 22px; }
            button { font-size: 14px; padding: 8px 12px; }
        }

        @media (max-width: 768px) {
            h2 { font-size: 20px; }
            button { font-size: 12px; padding: 6px 10px; }
            .note-buttons { gap: 5px; }
        }

        @media (max-width: 480px) {
            h2 { font-size: 18px; }
            button { font-size: 10px; padding: 5px 8px; }
            .note-buttons { gap: 3px; }
        }
    </style>
</head>
<body>
    <h2>Music Notation Shuffle</h2>
    <label for="notation">Select Notation:</label>
    <select id="notation-select">
        <option value="C,D,E">C, D, E</option>
        <option value="Do,Re,Mi">Do, Re, Mi</option>
    </select>
    <br><br>
    <button id="shuffle-button">Shuffle</button>
    <div id="notation-area" class="note-buttons"></div>
    <div class="message" id="message"></div>

    <script src="script.js"></script>
</body>
</html>
