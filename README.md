<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Image Puzzle</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="puzzle-container">
        <!-- 16 pieces for the puzzle -->
        <div class="puzzle1_A.jpg" data-order="1"></div>
        <div class="piece p2" data-order="2"></div>
        <div class="piece p3" data-order="3"></div>
        <div class="piece p4" data-order="4"></div>
        <div class="piece p5" data-order="5"></div>
        <div class="piece p6" data-order="6"></div>
        <div class="piece p7" data-order="7"></div>
        <div class="piece p8" data-order="8"></div>
        <div class="piece p9" data-order="9"></div>
        <div class="piece p10" data-order="10"></div>
        <div class="piece p11" data-order="11"></div>
        <div class="piece p12" data-order="12"></div>
        <div class="piece p13" data-order="13"></div>
        <div class="piece p14" data-order="14"></div>
        <div class="piece p15" data-order="15"></div>
        <div class="piece p16" data-order="16"></div>
        <!-- The extra piece that doesn't belong -->
        <div class="piece extra-piece" data-order="17"></div>
    </div>
</body>
body {
    font-family: sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #f0f0f0;
}

#puzzle-container {
    display: flex;
    flex-wrap: wrap; /* Allows items to wrap to new lines */
    width: 312px; /* Adjust based on image size (3 * 100px + gap) */
    height: 312px;
    gap: 4px; /* Space between puzzle pieces */
    border: 2px solid #333;
    padding: 4px;
    background-color: #fff;
}

.puzzle-piece {
    width: 100px;
    height: 100px;
    cursor: pointer;
    box-sizing: border-box;
    /* transition: transform 0.2s; Optional: adds a smooth effect when selected */
}

.puzzle-piece.selected {
    border: 3px solid blue; /* Highlight selected pieces */
}

#shuffle-btn {
    margin-top: 20px;
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
}
</html>
