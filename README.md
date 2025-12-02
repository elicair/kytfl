<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox 4x4 Image Grid</title>
    <style>
        /* Basic reset for consistent sizing */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: sans-serif;
        }

        .grid-container {
            display: flex;
            flex-wrap: wrap; /* Allows items to wrap to the next line */
            justify-content: space-between; /* Distributes space between items horizontally */
            gap: 10px; /* Provides consistent spacing between grid items */
            padding: 10px;
            max-width: 800px; /* Optional: Sets a max width for the grid area */
            margin: 20px auto; /* Centers the grid on the page */
        }

        .grid-item {
            /* 100% / 4 items = 25% width per item */
            /* Using calc() subtracts the gap space to prevent overflow */
            flex-basis: calc(25% - 8px); 
            flex-grow: 1; /* Allows items to grow slightly to fill the row perfectly */
            position: relative;
            overflow: hidden;
            /* Creates a square container using the padding-top trick */
            padding-top: 25%; 
            height: 0;
            border: 1px solid #ccc;
        }

        .grid-item img {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover; /* Ensures images cover the area without stretching */
            display: block;
        }
    </style>
</head>
<body>

    <div class="grid-container">
        <div class="grid-item"><img src="puzzle1_M.jpg" alt="Image 1"></div>
        <div class="grid-item"><img src="puzzle1_Q.jpg" alt="Image 2"></div>
        <div class="grid-item"><img src="puzzle1_J.jpg" alt="Image 3"></div>
        <div class="grid-item"><img src="puzzle1_G.jpg" alt="Image 4"></div>
        <div class="grid-item"><img src="puzzle1_A.jpg" alt="Image 5"></div>
        <div class="grid-item"><img src="puzzle1_B.jpg" alt="Image 6"></div>
        <div class="grid-item"><img src="puzzle1_H.jpg" alt="Image 7"></div>
        <div class="grid-item"><img src="puzzle1_P.jpg" alt="Image 8"></div>
        <div class="grid-item"><img src="puzzle1_E.jpg" alt="Image 9"></div>
        <div class="grid-item"><img src="puzzle1_N.jpg" alt="Image 10"></div>
        <div class="grid-item"><img src="puzzle1_C.jpg" alt="Image 11"></div>
        <div class="grid-item"><img src="puzzle1_O.jpg" alt="Image 12"></div>
        <div class="grid-item"><img src="puzzle1_F.jpg" alt="Image 13"></div>
        <div class="grid-item"><img src="puzzle1_L.jpg" alt="Image 14"></div>
        <div class="grid-item"><img src="puzzle1_K.jpg" alt="Image 15"></div>
        <div class="grid-item"><img src="puzzle1_I.jpg" alt="Image 16"></div>
    </div>
