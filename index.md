---
layout: default
title: "Static Bingo"
fulltitle: "Da Static - Static Bingo" 
excerpt: This is the greatest bingo website on earth. I'm dead inside!
---

<style>
    @import url(https://fonts.googleapis.com/css?family=Roboto:400,700);

    * {
        border: 0;
        margin: 0;
        outline: 0;
        padding: 0;
    }
    
    html, body {
        height: 100vh;
        width: 100vw;
    }

    body {
        background: #262522;
    }
    
    @media only screen and (min-width: 768px) {
        body {
            background: #262522 url(https://github.com/RichardPreziosi/StaticBingo/blob/main/tv.jpeg?raw=true) no-repeat center;
            -webkit-background-size: 265%;
            -moz-background-size: 265%;
            -o-background-size: 265%;
            background-size: 265%;
        }
    }

    @media only screen and (min-width: 1024px) {
        body {
            -webkit-background-size: 200%;
            -moz-background-size: 200%;
            -o-background-size: 200%;
            background-size: 200%;
        }
    }

    @media only screen and (min-width: 1440px) {
        body {
            -webkit-background-size: 150%;
            -moz-background-size: 150%;
            -o-background-size: 150%;
            background-size: 150%;
        }
    }

    @media only screen and (min-width: 2560px) {
        body {
            -webkit-background-size: 80%;
            -moz-background-size: 80%;
            -o-background-size: 80%;
            background-size: 80%;
        }
    }
    
    #wrapper {
        left: 50%;
        margin: auto;
        margin: 0;
        position: absolute;
        top: 50%;
        transform: translate(-50%, -50%);
        width: 640px;
    }

    #card {
        color: #fff;
        margin: 0 auto;
        position: absolute;
        text-align: center;
        display: grid;
        grid-gap: 10px;
        grid-template-rows: repeat(5, 80px);
        grid-template-columns: repeat(5, 100px);
    }

        #card > div {
            background: #393939;
            display: flex;
            align-items: center;
            text-align: center;
            justify-content: center;
            position: relative;
            cursor: pointer;
            user-select: none;
            box-sizing: border-box;
            padding: 5px;
            min-width: 0;
        }

            #card > div:hover {
                -moz-box-shadow: inset 0 0 35px rgba(187, 187, 187, 0.25);
                -moz-transition-duration: 0.25s;
                -o-transition-duration: 0.25s;
                -webkit-box-shadow: inset 0 0 35px rgba(187, 187, 187, 0.25);
                -webkit-transition-duration: 0.25s;
                box-shadow: inset 0 0 35px rgba(187, 187, 187, 0.25);
                transition-duration: 0.25s;
            }

            #card > div > span {
                display: block; /* Fallback for non-webkit */
                display: -webkit-box;
                margin: 0 auto;
                overflow: hidden;
                text-overflow: ellipsis;
                font: 14px arial;
                max-height: 70px;
                -webkit-line-clamp: 4;
                -webkit-box-orient: vertical;
            }

    #card .dabbedRed { background: #ff0000; }

    #card .dabbedBlue { background: #0000ff; }

    #card .dabbedYellow { background: #e6e607; }

    #card .dabbedGreen { background: #008000; }

    #card .dabbedPurple { background: #800080; }

    #card .dabbedOrange { background: #ffa500; }

    #card .dabbedBlack { background: #000000; }

    #menu {
        left: 560px;
        position: relative;
        width: 100px;
    }

    #menu #scoreboard {
        color: #fff;
        font: 12px roboto;
        height: 180px;
        text-align: center;
        width: 100px;
    }

    #menu #scoreboard .title {
        letter-spacing: 1px;
        padding-top: 9px;
    }

    #menu #scoreboard .score { font-size: 30px; }

    #menu .cardFunction {
        background: rgba(34, 34, 34, 0.6);
        color: #fff;
        font: 12px/45px roboto;
        height: 45px;
        margin-top: 10px;
        width: 100px;
        cursor: pointer;
    }

    #menu .cardFunction:hover {
        -moz-transition-duration: 0.25s;
        -o-transition-duration: 0.25s;
        -webkit-transition-duration: 0.25s;
        background: #222222;
        transition-duration: 0.25s;
    }

    #menu #palette {
        background: rgba(34, 34, 34, 0.6);
        color: white;
        font: 12px/28px roboto;
        margin-top: 10px;
        text-align: center;
    }

    #menu #palette .dabSelect {
        border-radius: 24px;
        float: left;
        height: 44px;
        margin: 0 0 4px 4px;
        vertical-align: top;
        width: 44px;
    }

    #menu #palette .dabSelect:hover { border: 3px solid #fff; }

    #menu #palette #dabRed { background: #ff0000; }

    #menu #palette #dabBlue { background: #0000ff; }

    #menu #palette #dabYellow { background: #e6e607; }

    #menu #palette #dabGreen { background: #008000; }

    #menu #palette #dabPurple { background: #800080; }

    #menu #palette #dabOrange { background: #ffa500; }

    #menu #palette #dabBlack { background: #000000; }

    #menu #palette #dabRandom {
        background: #ffffff;
        font: 20px roboto;
    }

    #menu #palette .dabActive { border: 3px solid #aaa; }

    #credit {
        font: 12px roboto;
        letter-spacing: 2px;
        margin-top: 10px;
        text-align: center;
        text-shadow: -1px -1px #888;
        width: 100%;
    }

    #credit a {
        color: #111;
        text-decoration: none;
    }

    #credit a:hover { text-shadow: 1px 1px #888; }

</style>

<div id="wrapper">
    <div id="card">
        <div id="cell0"><span></span></div>
        <div id="cell1"><span></span></div>
        <div id="cell2"><span></span></div>
        <div id="cell3"><span></span></div>
        <div id="cell4"><span></span></div>
        <div id="cell5"><span></span></div>
        <div id="cell6"><span></span></div>
        <div id="cell7"><span></span></div>
        <div id="cell8"><span></span></div>
        <div id="cell9"><span></span></div>
        <div id="cell10"><span></span></div>
        <div id="cell11"><span></span></div>
        <div id="cell12"><span></span></div>
        <div id="cell13"><span></span></div>
        <div id="cell14"><span></span></div>
        <div id="cell15"><span></span></div>
        <div id="cell16"><span></span></div>
        <div id="cell17"><span></span></div>
        <div id="cell18"><span></span></div>
        <div id="cell19"><span></span></div>
        <div id="cell20"><span></span></div>
        <div id="cell21"><span></span></div>
        <div id="cell22"><span></span></div>
        <div id="cell23"><span></span></div>
        <div id="cell24"><span></span></div>
    </div>
    <div id="menu">
        <div id="scoreboard">
            <p class="title">ROWS</p>
            <p class="score"><span id="scoreRow">0</span>/5</p>
            <p class="title">COLUMNS</p>
            <p class="score"><span id="scoreCol">0</span>/5</p>
            <p class="title">DIAGONALS</p>
            <p class="score"><span id="scoreDiag">0</span>/2</p>
        </div>
        <button class="cardFunction" id="newCard">NEW CARD</button>
        <button class="cardFunction" id="cleanCard">CLEAR</button>
        <div id="palette">
            <button class="dabSelect" id="dabRed"></button>
            <button class="dabSelect" id="dabBlue"></button>
            <button class="dabSelect" id="dabYellow"></button>
            <button class="dabSelect" id="dabGreen"></button>
            <button class="dabSelect" id="dabPurple"></button>
            <button class="dabSelect" id="dabOrange"></button>
        </div>
    </div>
</div>

<script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>

<script type="text/javascript">
    $(document).ready(function() {
        // Array containing all of the potential square content and their descriptions, separated by "::".
        var squares = [];
        var randomDab = ['dabbedRed', 'dabbedBlue', 'dabbedYellow', 'dabbedGreen', 'dabbedPurple', 'dabbedOrange', 'dabbedBlack'];
        var isDabbed = ['cell12'];
        var bingoRow = [];
        var bingoCol = [];
        var bingoDiagonal = [];
        var dabColor;

        // Function to shuffle/randomize array content
        function shuffle(v) {
            for (var j, x, i = v.length; i; j = parseInt(Math.random() * i, 10), x = v[--i], v[i] = v[j], v[j] = x);
            return v;
        }

        // Function to clear all dabs from the card
        function cleanCard() {
            $('#card > div').removeClass();
            isDabbed = [];
            bingoRow = [];
            bingoCol = [];
            bingoDiagonal = [];
            $('#scoreRow').html(bingoRow.length);
            $('#scoreCol').html(bingoCol.length);
            $('#scoreDiag').html(bingoDiagonal.length);
        }

        // Function to fill the card with randomized square entries
        function fillCard() {
            cleanCard();
            shuffle(squares);
            for (var i = 0; i < 25; i++) {
                var squareName = squares[i];
                $('#cell' + i + ' span').html(squareName).attr('title', squareName);
            }
        }

        // Function to give the customary free center dab
        function freeDab() {
            isDabbed.push('cell12');
            if (dabColor === 'random') {
                $('#cell12').addClass(randomDab[Math.floor(Math.random() * randomDab.length)]).html('Freebie!').attr('title', "");
            } else {
                $('#cell12').addClass(dabColor).html('Taylor doesn\'t have Swiftcast').attr('title', "");
            }
        }

        // Function to check for multiple values within an array
        function containsAll(needles, haystack) {
            for (var i = 0, len = needles.length; i < len; i++) {
                if ($.inArray(needles[i], haystack) === -1) return false;
            }
            return true;
        }

        // Function to check for bingos (by searching the isDabbed array for the right sequences of cells) then save them to the bingo array
        function bingoCheck() {
            // Check rows (cells 0-4, 5-9, 10-14, 15-19, and 20-24)
            for (var i = 0; i < 21; i += 5) {
                // If all of a row's cells are in the isDabbed array, and if that row isn't already in the bingo array, add it
                if (containsAll(["cell" + i, "cell" + (i + 1), "cell" + (i + 2), "cell" + (i + 3), "cell" + (i + 4)], isDabbed)) {
                    if ($.inArray("row" + i, bingoRow) === -1) {
                        bingoRow.push("row" + i);
                        $('#scoreRow').html(bingoRow.length);
                        alert("BINGO bitches! You filled out a row.");
                    }
                    // If all of a row's cells are no longer in the isDabbed array, and if that row is already in the bingo array, remove it
                } else {
                    if ($.inArray("row" + i, bingoRow) !== -1) {
                        bingoRow.splice($.inArray("row" + i, bingoRow), 1);
                        $('#scoreRow').html(bingoRow.length);
                    }
                }
            }

            // Check columns (cells 0-20, 1-21, 2-22, 3-23, and 4-24)
            for (var i = 0; i < 5; i++) {
                // If all of a column's cells are in the isDabbed array, and if that column isn't already in the bingo array, add it
                if (containsAll(["cell" + i, "cell" + (i + 5), "cell" + (i + 10), "cell" + (i + 15), "cell" + (i + 20)], isDabbed)) {
                    if ($.inArray("col" + i, bingoCol) === -1) {
                        bingoCol.push("col" + i);
                        $('#scoreCol').html(bingoCol.length);
                        alert("BINGO Bitches! You filled out a column.");
                    }
                    // If all of a column's cells are no longer in the isDabbed array, and if that column is already in the bingo array, remove it
                } else {
                    if ($.inArray("col" + i, bingoCol) !== -1) {
                        bingoCol.splice($.inArray("col" + i, bingoCol), 1);
                        $('#scoreCol').html(bingoCol.length);
                    }
                }
            }

            // Check forward diagonal (cells 0, 6, 12, 18, and 24)
            if (containsAll(["cell0", "cell6", "cell12", "cell18", "cell24"], isDabbed)) {
                if ($.inArray("diag0", bingoDiagonal) === -1) {
                    bingoDiagonal.push("diag0");
                    $('#scoreDiag').html(bingoDiagonal.length);
                    alert("Bingo bitches! You filled out a diagonal.");
                }
            } else {
                if ($.inArray("diag0", bingoDiagonal) !== -1) {
                    bingoDiagonal.splice($.inArray("diag0", bingoDiagonal), 1);
                    $('#scoreDiag').html(bingoDiagonal.length);
                }
            }

            // Check backward diagonal (cells 4, 8, 12, 16, and 20)
            if (containsAll(["cell4", "cell8", "cell12", "cell16", "cell20"], isDabbed)) {
                if ($.inArray("diag4", bingoDiagonal) === -1) {
                    bingoDiagonal.push("diag4");
                    $('#scoreDiag').html(bingoDiagonal.length);
                    alert("Bingo bitches! You filled out a diagonal.");
                }
            } else {
                if ($.inArray("diag4", bingoDiagonal) !== -1) {
                    bingoDiagonal.splice($.inArray("diag4", bingoDiagonal), 1);
                    $('#scoreDiag').html(bingoDiagonal.length);
                }
            }

            // Check for a full bingo of all 12 row/column/diagonal combinations
            if ((bingoRow.length === 5) && (bingoCol.length === 5) && (bingoDiagonal.length === 2)) {
                alert("WOW, we really sucked tonight!");
            }
        }

        // Function to switch the active dabbing color
        function switchDab(color, id) {
            dabColor = color;
            $('.dabSelect').removeClass('dabActive');
            $(id).addClass('dabActive');
        }

        // When clicking a 'td' element, (1) add/remove the 'dabbed' class, (2) add/remove its id to/from the isDabbed array, and (3) run a check for bingos
        $('#card > div:not(#cell12)').click(function() {
            if ($.inArray(this.id, isDabbed) !== -1) {
                isDabbed.splice($.inArray(this.id, isDabbed), 1);
                $(this).removeClass();
            } else {
                isDabbed.push(this.id);
                if (dabColor == 'random') {
                    $(this).addClass(randomDab[Math.floor(Math.random() * randomDab.length)]);
                } else {
                    $(this).addClass(dabColor);
                }
            }
            bingoCheck();
        });

        // Refill the card when clicking the "#newCard" button
        $('#newCard').click(function () {
            if (isDabbed.length > 1) {
                if (!confirm('You have already started this card, are you sure you want a new one?')) {
                    return;
                }
            }
            fillCard();
            freeDab();
        });

        // Clear all dabs from the card when clicking the "#cleanCard" button
        $('#cleanCard').click(function() {
            cleanCard();
            freeDab();
        });
        // Switch the dabbing color to red
        $('#dabRed').click(function() {
            switchDab('dabbedRed', this);
        });
        // Switch the dabbing color to blue
        $('#dabBlue').click(function() {
            switchDab('dabbedBlue', this);
        });
        // Switch the dabbing color to green
        $('#dabYellow').click(function() {
            switchDab('dabbedYellow', this);
        });
        // Switch the dabbing color to yellow
        $('#dabGreen').click(function() {
            switchDab('dabbedGreen', this);
        });
        // Switch the dabbing color to purple
        $('#dabPurple').click(function() {
            switchDab('dabbedPurple', this);
        });
        // Switch the dabbing color to orange
        $('#dabOrange').click(function() {
            switchDab('dabbedOrange', this);
        });
        // Switch the dabbing color to black
        $('#dabBlack').click(function() {
            switchDab('dabbedBlack', this);
        });
        // Switch the dabbing color to random
        $('#dabRandom').click(function() {
            switchDab('random', this);
        });

        // Initialize the card on page load
        $.get('https://raw.githubusercontent.com/RichardPreziosi/StaticBingo/main/items.txt',
                function (data) {
                    squares = data.match(/.+/g);
                    switchDab('dabbedRed', '#dabRed');
                    fillCard();
                    freeDab();
                }).fail(function() {
                    alert( "There was an error loading the squares!" );
                });
    });
</script>
