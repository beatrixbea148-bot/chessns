<!DOCTYPE html>
<html>
<head>
<title>Chess Academy</title>

<style>

body{
    margin:0;
    background:#262421;
    color:white;
    font-family:Arial,sans-serif;
}

header{
    background:#312e2b;
    padding:20px;
    text-align:center;
}

.hero{
    padding:50px;
    text-align:center;
}

.hero h1{
    font-size:48px;
}

.btn{
    background:#81b64c;
    color:white;
    padding:15px 30px;
    border:none;
    border-radius:8px;
    cursor:pointer;
    font-size:18px;
}

.courses{

    display:grid;

    grid-template-columns:
    repeat(auto-fit,minmax(300px,1fr));

    gap:20px;

    padding:20px;
}

.card{

    background:#312e2b;

    padding:20px;

    border-radius:10px;
}

.card h2{
    color:#81b64c;
}

a{
    color:white;
    text-decoration:none;
}

</style>

</head>
<body>

<header>

<h1>♟ Chess Academy</h1>

<p>Learn Chess From Beginner To Advanced</p>

</header>

<section class="hero">

<h1>Master Chess Step By Step</h1>

<p>

Lessons • Puzzles • Openings • Analysis

</p>

<button class="btn">

Start Learning

</button>

</section>

<section class="courses">

<div class="card">

<h2>🌱 Beginner</h2>

<ul>

<li>Board Setup</li>
<li>How Pieces Move</li>
<li>Check & Checkmate</li>
<li>Castling</li>
<li>En Passant</li>

</ul>

</div>

<div class="card">

<h2>⚔ Intermediate</h2>

<ul>

<li>Opening Principles</li>
<li>Forks</li>
<li>Pins</li>
<li>Skewers</li>
<li>Basic Endgames</li>

</ul>

</div>

<div class="card">

<h2>🚀 Advanced</h2>

<ul>

<li>Opening Theory</li>
<li>Positional Play</li>
<li>Calculation</li>
<li>Advanced Endgames</li>
<li>Classical Games</li>

</ul>

</div>

</section>

</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Chess Academy</title>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.css">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:Arial,sans-serif;
background:#262421;
color:white;
}

header{
background:#312e2b;
padding:20px;
text-align:center;
}

header h1{
font-size:40px;
color:#81b64c;
}

nav{
background:#1f1d1b;
padding:15px;
display:flex;
justify-content:center;
flex-wrap:wrap;
gap:20px;
}

nav a{
color:white;
text-decoration:none;
font-weight:bold;
}

.hero{
text-align:center;
padding:50px 20px;
}

.hero h2{
font-size:42px;
margin-bottom:15px;
}

.hero p{
font-size:20px;
margin-bottom:20px;
}

.btn{
background:#81b64c;
padding:12px 25px;
border:none;
border-radius:8px;
color:white;
cursor:pointer;
font-size:18px;
}

.container{
max-width:1200px;
margin:auto;
padding:20px;
}

.card{
background:#312e2b;
padding:20px;
border-radius:12px;
margin-bottom:20px;
}

.card h2{
color:#81b64c;
margin-bottom:15px;
}

.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
gap:20px;
}

#board{
width:100%;
max-width:600px;
margin:auto;
}

iframe{
width:100%;
height:300px;
border:none;
border-radius:10px;
}

.progress{
background:#1f1d1b;
height:25px;
border-radius:20px;
overflow:hidden;
}

.progress-fill{
height:100%;
width:35%;
background:#81b64c;
}

footer{
text-align:center;
padding:20px;
background:#1f1d1b;
margin-top:30px;
}

</style>
</head>
<body>

<header>

<h1>♟ Chess Academy</h1>

<p>Learn Chess From Beginner To Advanced</p>

</header>

<nav>

<a href="#learn">Learn</a>
<a href="#puzzles">Puzzles</a>
<a href="#board-section">Practice</a>
<a href="#openings">Openings</a>
<a href="#videos">Videos</a>
<a href="#progress">Progress</a>

</nav>

<section class="hero">

<h2>Master Chess Step By Step</h2>

<p>
Lessons • Puzzles • Openings • Analysis • Practice
</p>

<button class="btn">
Start Learning
</button>

</section>

<div class="container">

<section id="learn" class="card">

<h2>📚 Learning Path</h2>

<div class="grid">

<div>
<h3>🌱 Beginner</h3>
<ul>
<li>Board Setup</li>
<li>Piece Movement</li>
<li>Check & Checkmate</li>
<li>Castling</li>
<li>En Passant</li>
</ul>
</div>

<div>
<h3>⚔ Intermediate</h3>
<ul>
<li>Opening Principles</li>
<li>Forks</li>
<li>Pins</li>
<li>Skewers</li>
<li>Basic Endgames</li>
</ul>
</div>

<div>
<h3>🚀 Advanced</h3>
<ul>
<li>Opening Theory</li>
<li>Calculation</li>
<li>Positional Play</li>
<li>Advanced Endgames</li>
<li>Classical Games</li>
</ul>
</div>

</div>

</section>

<section id="puzzles" class="card">

<h2>🧩 Daily Puzzle</h2>

<p>
White to move and checkmate in 1.
</p>

<button class="btn">
Load Puzzle
</button>

</section>

<section id="board-section" class="card">

<h2>♟ Practice Board</h2>

<div id="board"></div>

</section>

<section id="openings" class="card">

<h2>📖 Opening Explorer</h2>

<h3>Italian Game</h3>
<p>1.e4 e5 2.Nf3 Nc6 3.Bc4</p>

<h3>Ruy Lopez</h3>
<p>1.e4 e5 2.Nf3 Nc6 3.Bb5</p>

<h3>Queen's Gambit</h3>
<p>1.d4 d5 2.c4</p>

<h3>Sicilian Defense</h3>
<p>1.e4 c5</p>

</section>

<section id="videos" class="card">

<h2>📺 Video Tutorials</h2>

<div class="grid">

<div>
<h3>Beginner</h3>
<iframe
src="https://www.youtube.com/embed/OCSbzArwB10"
allowfullscreen>
</iframe>
</div>

<div>
<h3>Intermediate</h3>
<iframe
src="https://www.youtube.com/embed/yv7_5JjP7GA"
allowfullscreen>
</iframe>
</div>

<div>
<h3>Advanced</h3>
<iframe
src="https://www.youtube.com/embed/U2huVf1l4UE"
allowfullscreen>
</iframe>
</div>

</div>

</section>

<section id="progress" class="card">

<h2>🏆 Progress</h2>

<p>Lessons Completed: 7 / 20</p>

<div class="progress">
<div class="progress-fill"></div>
</div>

<br>

<h3>Achievements</h3>

<ul>
<li>🥉 First Lesson</li>
<li>🥈 Puzzle Solver</li>
<li>🥇 Opening Student</li>
</ul>

</section>

</div>

<footer>

<p>♟ Chess Academy © 2026</p>

</footer>

<script src="https://cdnjs.cloudflare.com/ajax/libs/chess.js/0.13.4/chess.min.js"></script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.js"></script>

<script>

const board = Chessboard('board',{

position:'start',

draggable:true,

pieceTheme:
'https://images.chesscomfiles.com/chess-themes/pieces/neo/150/{piece}.png'

});

</script>

</body>
</html>
<section id="videos">

<h2>📺 Chess Video Academy</h2>

<!-- BEGINNER -->

<div class="tier">

<h2>🌱 Beginner Course</h2>

<p>
Learn the rules and fundamentals before studying openings.
</p>

<div class="video-grid">

<iframe
src="https://www.youtube.com/embed?listType=user_uploads&list=BiyaherongChessCoach"
allowfullscreen>
</iframe>

<iframe
src="https://www.youtube.com/embed?listType=user_uploads&list=BiyaherongChessCoach"
allowfullscreen>
</iframe>

<iframe
src="https://www.youtube.com/embed?listType=user_uploads&list=BiyaherongChessCoach"
allowfullscreen>
</iframe>

</div>

</div>

<!-- INTERMEDIATE -->

<div class="tier">

<h2>⚔ Intermediate Course</h2>

<p>
Forks, pins, skewers, combinations and planning.
</p>

<div class="video-grid">

<iframe
src="https://www.youtube.com/embed?listType=user_uploads&list=BiyaherongChessCoach"
allowfullscreen>
</iframe>

<iframe
src="https://www.youtube.com/embed?listType=user_uploads&list=BiyaherongChessCoach"
allowfullscreen>
</iframe>

<iframe
src="https://www.youtube.com/embed?listType=user_uploads&list=BiyaherongChessCoach"
allowfullscreen>
</iframe>

</div>

</div>

<!-- ADVANCED -->

<div class="tier">

<h2>🚀 Advanced Course</h2>

<p>
Opening theory, endgames and grandmaster game analysis.
</p>

<div class="video-grid">

<iframe
src="https://www.youtube.com/embed?listType=user_uploads&list=BiyaherongChessCoach"
allowfullscreen>
</iframe>

<iframe
src="https://www.youtube.com/embed?listType=user_uploads&list=BiyaherongChessCoach"
allowfullscreen>
</iframe>

<iframe
src="https://www.youtube.com/embed?listType=user_uploads&list=BiyaherongChessCoach"
allowfullscreen>
</iframe>

</div>

</div>

</section>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Beginner Chess Course</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:Arial,sans-serif;
background:#262421;
color:white;
}

header{
background:#312e2b;
padding:20px;
text-align:center;
}

header h1{
color:#81b64c;
}

nav{
background:#1f1d1b;
padding:15px;
text-align:center;
}

nav a{
color:white;
text-decoration:none;
margin:10px;
font-weight:bold;
}

.container{
max-width:1200px;
margin:auto;
padding:20px;
}

.card{
background:#312e2b;
padding:20px;
border-radius:12px;
margin-bottom:20px;
}

.card h2{
color:#81b64c;
margin-bottom:10px;
}

.video-grid{
display:grid;
grid-template-columns:
repeat(auto-fit,minmax(320px,1fr));
gap:20px;
}

iframe{
width:100%;
height:220px;
border:none;
border-radius:10px;
}

button{
background:#81b64c;
color:white;
border:none;
padding:12px 20px;
border-radius:6px;
cursor:pointer;
}

.progress{
background:#1f1d1b;
height:25px;
border-radius:20px;
overflow:hidden;
}

.progress-fill{
background:#81b64c;
height:100%;
width:20%;
}

.lesson-list li{
margin-bottom:8px;
}

footer{
background:#1f1d1b;
padding:20px;
text-align:center;
}

</style>
</head>
<body>

<header>

<h1>🌱 Beginner Chess Course</h1>

<p>Learn Chess From Absolute Beginner</p>

</header>

<nav>

<a href="index.html">Home</a>
<a href="#lessons">Lessons</a>
<a href="#videos">Videos</a>
<a href="#puzzle">Puzzle</a>

</nav>

<div class="container">

<section id="lessons" class="card">

<h2>📚 Beginner Lessons</h2>

<ul class="lesson-list">

<li>✅ Board Setup</li>

<li>✅ How Pawns Move</li>

<li>✅ How Knights Move</li>

<li>✅ How Bishops Move</li>

<li>✅ How Rooks Move</li>

<li>✅ How Queens Move</li>

<li>✅ How Kings Move</li>

<li>✅ Check</li>

<li>✅ Checkmate</li>

<li>✅ Stalemate</li>

<li>✅ Castling</li>

<li>✅ En Passant</li>

<li>✅ Pawn Promotion</li>

<li>✅ Opening Principles</li>

</ul>

</section>

<section class="card">

<h2>📖 Opening Principles</h2>

<ul>

<li>Control the center.</li>

<li>Develop your pieces.</li>

<li>Castle early.</li>

<li>Don't move the queen too early.</li>

<li>Connect your rooks.</li>

</ul>

</section>

<section id="videos" class="card">

<h2>📺 Beginner Video Lessons</h2>

<div class="video-grid">

<div>

<h3>Lesson 1</h3>

<iframe
src="https://www.youtube.com/embed/VIDEO_ID_1"
allowfullscreen>
</iframe>

</div>

<div>

<h3>Lesson 2</h3>

<iframe
src="https://www.youtube.com/embed/VIDEO_ID_2"
allowfullscreen>
</iframe>

</div>

<div>

<h3>Lesson 3</h3>

<iframe
src="https://www.youtube.com/embed/VIDEO_ID_3"
allowfullscreen>
</iframe>

</div>

</div>

</section>

<section id="puzzle" class="card">

<h2>🧩 Beginner Puzzle</h2>

<p>

White to move and checkmate in one move.

</p>

<pre>

Black King: g8

White Queen: f7

White King: g6

White to move

</pre>

<button onclick="showAnswer()">

Show Answer

</button>

<p id="answer"></p>

</section>

<section class="card">

<h2>🏆 Beginner Progress</h2>

<p>

Lessons Completed: 3 / 14

</p>

<div class="progress">

<div class="progress-fill"></div>

</div>

<br>

<h3>Achievements</h3>

<ul>

<li>🥉 First Lesson</li>

<li>🥉 Learned Piece Movement</li>

<li>🥈 First Puzzle Solved</li>

</ul>

</section>

<section class="card">

<h2>🎯 Beginner Goals</h2>

<ul>

<li>Know all chess rules.</li>

<li>Understand checkmate.</li>

<li>Learn opening principles.</li>

<li>Solve simple puzzles.</li>

<li>Play complete games.</li>

</ul>

</section>

</div>

<footer>

♟ Chess Academy Beginner Course

</footer>

<script>

function showAnswer(){

document.getElementById(
"answer"
).innerHTML =
"✅ Solution: Qg7#";

}

</script>

</body>
</html
 <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Intermediate Chess Course</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:Arial,sans-serif;
background:#262421;
color:white;
}

header{
background:#312e2b;
padding:20px;
text-align:center;
}

header h1{
color:#81b64c;
}

nav{
background:#1f1d1b;
padding:15px;
text-align:center;
}

nav a{
color:white;
text-decoration:none;
margin:10px;
font-weight:bold;
}

.container{
max-width:1200px;
margin:auto;
padding:20px;
}

.card{
background:#312e2b;
padding:20px;
border-radius:12px;
margin-bottom:20px;
}

.card h2{
color:#81b64c;
margin-bottom:15px;
}

.video-grid{
display:grid;
grid-template-columns:
repeat(auto-fit,minmax(320px,1fr));
gap:20px;
}

iframe{
width:100%;
height:220px;
border:none;
border-radius:10px;
}

button{
background:#81b64c;
color:white;
border:none;
padding:12px 20px;
border-radius:6px;
cursor:pointer;
}

.progress{
background:#1f1d1b;
height:25px;
border-radius:20px;
overflow:hidden;
}

.progress-fill{
background:#81b64c;
height:100%;
width:50%;
}

.lesson-list li{
margin-bottom:8px;
}

pre{
background:#1f1d1b;
padding:10px;
border-radius:8px;
overflow:auto;
}

footer{
background:#1f1d1b;
padding:20px;
text-align:center;
}

</style>
</head>
<body>

<header>

<h1>⚔ Intermediate Chess Course</h1>

<p>Tactics • Strategy • Openings • Endgames</p>

</header>

<nav>

<a href="index.html">Home</a>
<a href="#lessons">Lessons</a>
<a href="#openings">Openings</a>
<a href="#videos">Videos</a>
<a href="#puzzle">Puzzle</a>

</nav>

<div class="container">

<section id="lessons" class="card">

<h2>📚 Intermediate Lessons</h2>

<ul class="lesson-list">

<li>✅ Forks</li>
<li>✅ Pins</li>
<li>✅ Skewers</li>
<li>✅ Discovered Attacks</li>
<li>✅ Double Attacks</li>
<li>✅ Deflection</li>
<li>✅ Decoy</li>
<li>✅ Removing the Defender</li>
<li>✅ Basic Strategy</li>
<li>✅ Piece Activity</li>
<li>✅ Weak Squares</li>
<li>✅ Open Files</li>
<li>✅ Basic Endgames</li>

</ul>

</section>

<section id="openings" class="card">

<h2>📖 Opening Repertoire</h2>

<h3>Italian Game</h3>

<pre>
1.e4 e5
2.Nf3 Nc6
3.Bc4
</pre>

<h3>Queen's Gambit</h3>

<pre>
1.d4 d5
2.c4
</pre>

<h3>London System</h3>

<pre>
1.d4 d5
2.Bf4
</pre>

<h3>Caro-Kann Defense</h3>

<pre>
1.e4 c6
</pre>

</section>

<section class="card">

<h2>🎯 Tactical Themes</h2>

<ul>

<li>Knight Forks</li>
<li>Bishop Pins</li>
<li>Queen Skewers</li>
<li>Back Rank Mates</li>
<li>Smothered Mates</li>
<li>Greek Gift Sacrifice</li>

</ul>

</section>

<section id="videos" class="card">

<h2>📺 Intermediate Video Lessons</h2>

<div class="video-grid">

<div>

<h3>Forks & Tactics</h3>

<iframe
src="https://www.youtube.com/embed/VIDEO_ID_1"
allowfullscreen>
</iframe>

</div>

<div>

<h3>Strategy</h3>

<iframe
src="https://www.youtube.com/embed/VIDEO_ID_2"
allowfullscreen>
</iframe>

</div>

<div>

<h3>Opening Principles</h3>

<iframe
src="https://www.youtube.com/embed/VIDEO_ID_3"
allowfullscreen>
</iframe>

</div>

</div>

</section>

<section id="puzzle" class="card">

<h2>🧩 Tactical Puzzle</h2>

<p>
White to move and win material.
</p>

<pre>
Look for a tactical fork.
</pre>

<button onclick="showAnswer()">

Show Answer

</button>

<p id="answer"></p>

</section>

<section class="card">

<h2>🏆 Intermediate Progress</h2>

<p>

Lessons Completed: 10 / 20

</p>

<div class="progress">

<div class="progress-fill"></div>

</div>

<br>

<h3>Achievements</h3>

<ul>

<li>🥈 Tactical Student</li>
<li>🥈 Opening Explorer</li>
<li>🥈 Endgame Apprentice</li>

</ul>

</section>

<section class="card">

<h2>🎯 Intermediate Goals</h2>

<ul>

<li>Solve tactical puzzles daily.</li>
<li>Build an opening repertoire.</li>
<li>Understand basic strategy.</li>
<li>Master elementary endgames.</li>
<li>Analyze your games.</li>

</ul>

</section>

</div>

<footer>

♟ Chess Academy Intermediate Course

</footer>

<script>

function showAnswer(){

document.getElementById(
"answer"
).innerHTML =
"✅ Look for a knight fork attacking the king and queen.";

}

</script>

</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Advanced Chess Course</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:Arial,sans-serif;
background:#262421;
color:white;
}

header{
background:#312e2b;
padding:20px;
text-align:center;
}

header h1{
color:#81b64c;
}

nav{
background:#1f1d1b;
padding:15px;
text-align:center;
}

nav a{
color:white;
text-decoration:none;
margin:10px;
font-weight:bold;
}

.container{
max-width:1200px;
margin:auto;
padding:20px;
}

.card{
background:#312e2b;
padding:20px;
border-radius:12px;
margin-bottom:20px;
}

.card h2{
color:#81b64c;
margin-bottom:15px;
}

.video-grid{
display:grid;
grid-template-columns:
repeat(auto-fit,minmax(320px,1fr));
gap:20px;
}

iframe{
width:100%;
height:220px;
border:none;
border-radius:10px;
}

button{
background:#81b64c;
color:white;
border:none;
padding:12px 20px;
border-radius:6px;
cursor:pointer;
}

.progress{
background:#1f1d1b;
height:25px;
border-radius:20px;
overflow:hidden;
}

.progress-fill{
background:#81b64c;
height:100%;
width:80%;
}

.lesson-list li{
margin-bottom:8px;
}

pre{
background:#1f1d1b;
padding:10px;
border-radius:8px;
overflow:auto;
}

footer{
background:#1f1d1b;
padding:20px;
text-align:center;
}

</style>
</head>
<body>

<header>

<h1>🚀 Advanced Chess Course</h1>

<p>Master-Level Openings • Strategy • Endgames • Analysis</p>

</header>

<nav>

<a href="index.html">Home</a>
<a href="#lessons">Lessons</a>
<a href="#openings">Openings</a>
<a href="#games">Classical Games</a>
<a href="#videos">Videos</a>
<a href="#puzzle">Puzzle</a>

</nav>

<div class="container">

<section id="lessons" class="card">

<h2>📚 Advanced Lessons</h2>

<ul class="lesson-list">

<li>✅ Calculation Training</li>
<li>✅ Candidate Moves</li>
<li>✅ Positional Sacrifices</li>
<li>✅ Pawn Structures</li>
<li>✅ Prophylaxis</li>
<li>✅ Weak Squares</li>
<li>✅ Initiative</li>
<li>✅ Dynamic Imbalances</li>
<li>✅ Advanced Endgames</li>
<li>✅ Grandmaster Thinking Process</li>

</ul>

</section>

<section id="openings" class="card">

<h2>📖 Advanced Opening Theory</h2>

<h3>Ruy Lopez</h3>

<pre>
1.e4 e5
2.Nf3 Nc6
3.Bb5
</pre>

<h3>Main Variations</h3>

<ul>
<li>Berlin Defense</li>
<li>Marshall Attack</li>
<li>Closed Ruy Lopez</li>
<li>Open Ruy Lopez</li>
</ul>

<hr>

<h3>Sicilian Defense</h3>

<pre>
1.e4 c5
</pre>

<ul>
<li>Najdorf</li>
<li>Dragon</li>
<li>Classical</li>
<li>Sveshnikov</li>
</ul>

<hr>

<h3>French Defense</h3>

<pre>
1.e4 e6
2.d4 d5
</pre>

<ul>
<li>Winawer</li>
<li>Tarrasch</li>
<li>Advance Variation</li>
</ul>

</section>

<section id="games" class="card">

<h2>🏆 Classical Games To Study</h2>

<ul>

<li>Opera Game - Paul Morphy</li>

<li>Immortal Game - Anderssen</li>

<li>Evergreen Game - Anderssen</li>

<li>Game of the Century - Bobby Fischer</li>

<li>Kasparov vs Topalov (1999)</li>

<li>Capablanca Endgame Masterpieces</li>

</ul>

</section>

<section class="card">

<h2>♚ Advanced Endgames</h2>

<ul>

<li>Lucena Position</li>

<li>Philidor Position</li>

<li>Rook Endgames</li>

<li>Queen Endgames</li>

<li>Bishop vs Knight</li>

<li>Opposition</li>

<li>Triangulation</li>

</ul>

</section>

<section id="videos" class="card">

<h2>📺 Advanced Video Lessons</h2>

<div class="video-grid">

<div>

<h3>Advanced Opening Theory</h3>

<iframe
src="https://www.youtube.com/embed/VIDEO_ID_1"
allowfullscreen>
</iframe>

</div>

<div>

<h3>Positional Chess</h3>

<iframe
src="https://www.youtube.com/embed/VIDEO_ID_2"
allowfullscreen>
</iframe>

</div>

<div>

<h3>Grandmaster Analysis</h3>

<iframe
src="https://www.youtube.com/embed/VIDEO_ID_3"
allowfullscreen>
</iframe>

</div>

</div>

</section>

<section id="puzzle" class="card">

<h2>🧩 Advanced Puzzle</h2>

<p>

White to move and find the winning combination.

</p>

<pre>
Look for a forcing sequence.
Checks → Captures → Threats
</pre>

<button onclick="showAnswer()">

Show Solution Idea

</button>

<p id="answer"></p>

</section>

<section class="card">

<h2>🏆 Advanced Progress</h2>

<p>

Lessons Completed: 24 / 30

</p>

<div class="progress">

<div class="progress-fill"></div>

</div>

<br>

<h3>Achievements</h3>

<ul>

<li>🥇 Opening Expert</li>

<li>🥇 Tactical Master</li>

<li>🥇 Endgame Specialist</li>

<li>🏆 Advanced Student</li>

</ul>

</section>

<section class="card">

<h2>🎯 Advanced Goals</h2>

<ul>

<li>Create a complete opening repertoire.</li>

<li>Analyze your own games.</li>

<li>Master key endgames.</li>

<li>Study classical games regularly.</li>

<li>Improve calculation depth.</li>

<li>Understand strategic planning.</li>

</ul>

</section>

</div>

<footer>

♟ Chess Academy Advanced Course

</footer>

<script>

function showAnswer(){

document.getElementById(
"answer"
).innerHTML =
"✅ Start by looking at forcing checks. Calculate every response before choosing a move.";

}

</script>

</body>
</html>
VIDEO_ID_1
VIDEO_ID_2
VIDEO_ID_3
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Chess Academy - Puzzles</title>

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.css">

<style>

body{
    margin:0;
    background:#262421;
    color:white;
    font-family:Arial,sans-serif;
}

header{
    background:#312e2b;
    padding:20px;
    text-align:center;
}

header h1{
    color:#81b64c;
}

.container{
    max-width:1200px;
    margin:auto;
    padding:20px;
}

.card{
    background:#312e2b;
    padding:20px;
    border-radius:10px;
    margin-bottom:20px;
}

#board{
    width:min(90vw,600px);
    margin:auto;
}

button{
    padding:12px 20px;
    border:none;
    border-radius:6px;
    cursor:pointer;
    margin:5px;
    background:#81b64c;
    color:white;
}

select{
    padding:10px;
    border-radius:5px;
}

#status{
    margin-top:15px;
    font-size:20px;
    font-weight:bold;
}

#score{
    color:#81b64c;
    font-size:18px;
}

.white-1e1d7{
    background:#f0d9b5 !important;
}

.black-3c85d{
    background:#b58863 !important;
}

</style>
</head>
<body>

<header>

<h1>🧩 Chess Puzzle Trainer</h1>

<p>Solve puzzles and improve your tactics</p>

</header>

<div class="container">

<div class="card">

<h2>Select Difficulty</h2>

<select id="difficulty">

<option value="beginner">
Beginner
</option>

<option value="intermediate">
Intermediate
</option>

<option value="advanced">
Advanced
</option>

</select>

<button onclick="loadPuzzle()">
Load Puzzle
</button>

<button onclick="showHint()">
Hint
</button>

</div>

<div class="card">

<div id="board"></div>

<div id="status">
Choose a puzzle to begin.
</div>

</div>

<div class="card">

<h2>🏆 Progress</h2>

<p id="score">
Puzzles Solved: 0
</p>

</div>

</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/chess.js/0.13.4/chess.min.js"></script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.js"></script>

<script>

const game = new Chess();

let solved = 0;

let currentPuzzle = null;

const puzzles = {

beginner:[

{
title:"Mate in 1",
fen:"6k1/5Q2/6K1/8/8/8/8/8 w - - 0 1",
solution:"f7g7",
hint:"Use the queen."
}

],

intermediate:[

{
title:"Fork Tactic",
fen:"r3k2r/pppq1ppp/2n5/3Np3/8/8/PPP2PPP/R1BQK2R w KQkq - 0 1",
solution:"d5f6",
hint:"Knight fork."
}

],

advanced:[

{
title:"Winning Combination",
fen:"r2q1rk1/ppp2ppp/2n5/3Np3/8/8/PPP2PPP/R1BQ1RK1 w - - 0 1",
solution:"d5f6",
hint:"Find a forcing tactical move."
}

]

};

const board = Chessboard('board',{

draggable:true,

position:'start',

showNotation:true,

pieceTheme:
'https://images.chesscomfiles.com/chess-themes/pieces/neo/150/{piece}.png',

onDragStart:onDragStart,

onDrop:onDrop,

onSnapEnd:() => {

board.position(
game.fen()
);

}

});

function onDragStart(source,piece){

if(game.game_over())
return false;

if(
game.turn()==='w' &&
piece.search(/^b/) !== -1
)
return false;

if(
game.turn()==='b' &&
piece.search(/^w/) !== -1
)
return false;

}

function loadPuzzle(){

const level =
document.getElementById(
'difficulty'
).value;

const list =
puzzles[level];

currentPuzzle =
list[
Math.floor(
Math.random() *
list.length
)];

game.load(
currentPuzzle.fen
);

board.position(
game.fen()
);

document.getElementById(
'status'
).innerHTML =
'🎯 ' +
currentPuzzle.title;

}

function onDrop(source,target){

const move =
game.move({

from:source,
to:target,
promotion:'q'

});

if(move===null)
return 'snapback';

if(currentPuzzle){

const played =
source + target;

if(
played ===
currentPuzzle.solution
){

solved++;

document.getElementById(
'status'
).innerHTML =
'🎉 Puzzle Solved!';

document.getElementById(
'score'
).innerHTML =
'Puzzles Solved: ' +
solved;

currentPuzzle = null;

}
else{

document.getElementById(
'status'
).innerHTML =
'❌ Wrong Move';

game.undo();

return 'snapback';

}

}

}

function showHint(){

if(
!currentPuzzle
)return;

alert(
currentPuzzle.hint
);

}

window.addEventListener(
'resize',
()=>board.resize()
);

</script>

</body>
</html>
<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.css">

<script src="https://cdnjs.cloudflare.com/ajax/libs/chess.js/0.13.4/chess.min.js"></script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.js"></script>

<script src="stockfish.js"></script>
<div class="container">

<div id="board"></div>

<div class="sidebar">

<h2>♟ Play vs AI</h2>

<select id="difficulty">
<option value="1">Beginner</option>
<option value="5">Easy</option>
<option value="10">Medium</option>
<option value="15">Hard</option>
<option value="20">Extreme</option>
</select>

<div class="clock">
White: <span id="whiteTime">10:00</span>
</div>

<div class="clock">
Black: <span id="blackTime">10:00</span>
</div>

<div id="status"></div>

<div id="moves"></div>

<button onclick="newGame()">
New Game
</button>

</div>

</div>
const stockfish = new Worker("stockfish.js");

function makeAIMove(){

stockfish.postMessage(
"go depth 10"
);

stockfish.onmessage = function(event){

const line = event.data;

if(line.startsWith("bestmove")){

const move =
line.split(" ")[1];

game.move({
from: move.substring(0,2),
to: move.substring(2,4),
promotion: 'q'
});

board.position(
game.fen()
);

updateStatus();
}

};
}
let whiteSeconds = 600;
let blackSeconds = 600;

setInterval(() => {

if(game.turn() === 'w')
whiteSeconds--;

else
blackSeconds--;

updateClock();

},1000);
function updateMoves(){

const history =
game.history();

document
.getElementById("moves")
.innerHTML =
history.join("<br>");

}
let rating =
localStorage.getItem(
"rating"
) || 1200;

document.getElementById(
"rating"
).textContent =
rating;
highlightMove(
move.from,
move.to
);
stockfish.postMessage(
"position fen " +
game.fen()
);

stockfish.postMessage(
"go depth 15"
);
Evaluation: +1.5

Best Move:
Nf3

Accuracy:
92%
chess-academy/

index.html
beginner.html
intermediate.html
advanced.html
puzzles.html
play.html

css/
  style.css

js/
  play.js
  puzzles.js
  lessons.js

stockfish/
  stockfish.js

data/
  openings.json
  puzzles.json
  <!DOCTYPE html>
<html lang="en">
<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">

<title>Opening Explorer</title>

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.css">

<style>

body{
margin:0;
background:#262421;
color:white;
font-family:Arial,sans-serif;
}

header{
background:#312e2b;
padding:20px;
text-align:center;
}

header h1{
color:#81b64c;
}

.container{
max-width:1200px;
margin:auto;
padding:20px;
}

.card{
background:#312e2b;
padding:20px;
border-radius:10px;
margin-bottom:20px;
}

#board{
width:min(90vw,600px);
margin:auto;
}

select,
button{
padding:10px;
margin:5px;
border:none;
border-radius:6px;
font-size:16px;
}

button{
background:#81b64c;
color:white;
cursor:pointer;
}

.info{
line-height:1.7;
}

.move-box{
background:#1f1d1b;
padding:10px;
border-radius:8px;
margin-top:10px;
}

.white-1e1d7{
background:#f0d9b5 !important;
}

.black-3c85d{
background:#b58863 !important;
}

</style>

</head>

<body>

<header>

<h1>📖 Chess Opening Explorer</h1>

<p>
Study openings from Beginner to Advanced
</p>

</header>

<div class="container">

<div class="card">

<h2>Select Opening</h2>

<select id="openingSelect">

<option value="italian">
Italian Game
</option>

<option value="ruy">
Ruy Lopez
</option>

<option value="queens">
Queen's Gambit
</option>

<option value="sicilian">
Sicilian Defense
</option>

<option value="london">
London System
</option>

</select>

<button onclick="loadOpening()">
Load Opening
</button>

</div>

<div class="card">

<div id="board"></div>

<div style="text-align:center">

<button onclick="prevMove()">
⏮ Previous
</button>

<button onclick="nextMove()">
⏭ Next
</button>

</div>

</div>

<div class="card">

<h2 id="openingTitle">

Italian Game

</h2>

<div id="openingInfo" class="info">

Classic king pawn opening.

</div>

<div class="move-box">

<strong>Moves:</strong>

<div id="moveList">

1.e4 e5 2.Nf3 Nc6 3.Bc4

</div>

</div>

</div>

</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/chess.js/0.13.4/chess.min.js"></script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.js"></script>

<script>

const game = new Chess();

const board = Chessboard('board',{

position:'start',

pieceTheme:
'https://images.chesscomfiles.com/chess-themes/pieces/neo/150/{piece}.png'

});

const openings = {

italian:{

title:"Italian Game",

moves:[
"e4",
"e5",
"Nf3",
"Nc6",
"Bc4"
],

info:`
<b>Main Idea:</b><br>
Develop pieces quickly and attack f7.

<br><br>

<b>Opening Principles:</b>

<ul>

<li>Control the center</li>

<li>Develop knights before bishops</li>

<li>Castle early</li>

</ul>

<b>Common Plans:</b>

Attack kingside and create tactical opportunities.
`

},

ruy:{

title:"Ruy Lopez",

moves:[
"e4",
"e5",
"Nf3",
"Nc6",
"Bb5"
],

info:`
<b>Main Idea:</b>

Pressure the knight defending e5.

<br><br>

<b>Plans:</b>

<ul>

<li>Control center</li>

<li>Long-term pressure</li>

<li>Strong strategic positions</li>

</ul>
`

},

queens:{

title:"Queen's Gambit",

moves:[
"d4",
"d5",
"c4"
],

info:`
<b>Main Idea:</b>

Offer a pawn to gain center control.

<br><br>

<b>Plans:</b>

<ul>

<li>Strong pawn center</li>

<li>Queenside pressure</li>

<li>Positional play</li>

</ul>
`

},

sicilian:{

title:"Sicilian Defense",

moves:[
"e4",
"c5"
],

info:`
<b>Main Idea:</b>

Fight for the center asymmetrically.

<br><br>

<b>Plans:</b>

<ul>

<li>Counterattack</li>

<li>Dynamic positions</li>

<li>Winning chances for both sides</li>

</ul>
`

},

london:{

title:"London System",

moves:[
"d4",
"d5",
"Bf4"
],

info:`
<b>Main Idea:</b>

Simple setup with clear plans.

<br><br>

<b>Plans:</b>

<ul>

<li>Easy development</li>

<li>Solid structure</li>

<li>Beginner friendly</li>

</ul>
`

}

};

let currentMoves = [];
let moveIndex = 0;

function loadOpening(){

const selected =
document.getElementById(
'openingSelect'
).value;

const opening =
openings[selected];

document.getElementById(
'openingTitle'
).innerHTML =
opening.title;

document.getElementById(
'openingInfo'
).innerHTML =
opening.info;

document.getElementById(
'moveList'
).innerHTML =
opening.moves.join(' ');

currentMoves =
opening.moves;

moveIndex = 0;

game.reset();

board.position('start');

}

function nextMove(){

if(moveIndex >= currentMoves.length)
return;

game.move(
currentMoves[moveIndex]
);

board.position(
game.fen()
);

moveIndex++;

}

function prevMove(){

if(moveIndex <= 0)
return;

moveIndex--;

game.reset();

for(
let i=0;
i<moveIndex;
i++
){

game.move(
currentMoves[i]
);

}

board.position(
game.fen()
);

}

loadOpening();

</script>

</body>
</html>
stockfish/
└── stockfish.js
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">

<title>Chess Academy Analysis Board</title>

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.css">

<style>

body{
margin:0;
font-family:Arial,sans-serif;
background:#262421;
color:white;
}

header{
background:#312e2b;
padding:20px;
text-align:center;
}

header h1{
color:#81b64c;
}

.container{
display:flex;
flex-wrap:wrap;
gap:20px;
padding:20px;
justify-content:center;
}

#board{
width:min(90vw,700px);
}

.panel{
width:350px;
background:#312e2b;
padding:20px;
border-radius:10px;
}

.panel h2{
color:#81b64c;
margin-top:0;
}

textarea{
width:100%;
height:150px;
padding:10px;
border:none;
border-radius:6px;
resize:vertical;
}

button{
width:100%;
padding:12px;
margin-top:10px;
border:none;
border-radius:6px;
cursor:pointer;
background:#81b64c;
color:white;
font-size:16px;
}

.info-box{
background:#1f1d1b;
padding:10px;
border-radius:6px;
margin-top:10px;
}

#moves{
max-height:200px;
overflow:auto;
}

</style>

</head>
<body>

<header>

<h1>📊 Analysis Board</h1>

<p>
Analyze games with Stockfish
</p>

</header>

<div class="container">

<div id="board"></div>

<div class="panel">

<h2>Engine Analysis</h2>

<div class="info-box">

Evaluation:
<span id="eval">
0.00
</span>

</div>

<div class="info-box">

Best Move:
<span id="bestmove">
-
</span>

</div>

<div class="info-box">

Depth:
<span id="depth">
0
</span>

</div>

<button onclick="analyzePosition()">
Analyze Position
</button>

<button onclick="flipBoard()">
Flip Board
</button>

<button onclick="resetBoard()">
Reset Board
</button>

<h2>PGN Import</h2>

<textarea id="pgnInput"
placeholder="Paste PGN here..."></textarea>

<button onclick="loadPGN()">
Load PGN
</button>

<h2>Move List</h2>

<div id="moves"></div>

</div>

</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/chess.js/0.13.4/chess.min.js"></script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.js"></script>

<script>

const game = new Chess();

const board = Chessboard('board',{

draggable:true,

position:'start',

showNotation:true,

pieceTheme:
'https://images.chesscomfiles.com/chess-themes/pieces/neo/150/{piece}.png',

onDragStart:onDragStart,

onDrop:onDrop,

onSnapEnd:() => {

board.position(
game.fen()
);

}

});

function onDragStart(source,piece){

if(
(game.turn()==='w' &&
piece.search(/^b/)!==-1)
||
(game.turn()==='b' &&
piece.search(/^w/)!==-1)
)
return false;

}

function onDrop(source,target){

const move =
game.move({

from:source,
to:target,
promotion:'q'

});

if(move===null)
return 'snapback';

updateMoves();

}

function updateMoves(){

const history =
game.history();

let html='';

for(
let i=0;
i<history.length;
i+=2
){

html +=

(Math.floor(i/2)+1)
+ '. '
+ history[i];

if(history[i+1])
html +=
' '
+ history[i+1];

html += '<br>';

}

document
.getElementById('moves')
.innerHTML = html;

}

function flipBoard(){

board.flip();

}

function resetBoard(){

game.reset();

board.start();

updateMoves();

}

function loadPGN(){

const pgn =
document
.getElementById(
'pgnInput'
)
.value;

game.reset();

const loaded =
game.load_pgn(
pgn
);

if(!loaded){

alert(
'Invalid PGN'
);

return;

}

board.position(
game.fen()
);

updateMoves();

}

let stockfish = null;

try{

stockfish =
new Worker(
'stockfish/stockfish.js'
);

stockfish.onmessage =
function(event){

const line =
event.data;

if(
line.includes('depth')
){

const depthMatch =
line.match(
/depth (\d+)/
);

if(depthMatch){

document
.getElementById(
'depth'
)
.textContent =
depthMatch[1];

}

}

if(
line.includes('score cp')
){

const scoreMatch =
line.match(
/score cp (-?\d+)/
);

if(scoreMatch){

const evalScore =
(
parseInt(
scoreMatch[1]
)/100
).toFixed(2);

document
.getElementById(
'eval'
)
.textContent =
evalScore;

}

}

if(
line.startsWith(
'bestmove'
)
){

const move =
line.split(' ')[1];

document
.getElementById(
'bestmove'
)
.textContent =
move;

}

};

}
catch(e){

console.log(
'Stockfish not loaded'
);

}

function analyzePosition(){

if(!stockfish){

alert(
'Stockfish engine missing.'
);

return;

}

stockfish.postMessage(
'uci'
);

stockfish.postMessage(
'position fen '
+
game.fen()
);

stockfish.postMessage(
'go depth 18'
);

}

window.addEventListener(
'resize',
()=>board.resize()
);

updateMoves();

</script>

</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Play vs AI</title>

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.css">

<style>

body{
margin:0;
background:#262421;
color:white;
font-family:Arial,sans-serif;
}

header{
background:#312e2b;
padding:15px;
text-align:center;
}

header h1{
color:#81b64c;
margin:0;
}

.container{
display:flex;
flex-wrap:wrap;
justify-content:center;
gap:20px;
padding:20px;
}

#board{
width:min(90vw,650px);
}

.panel{
width:320px;
background:#312e2b;
padding:20px;
border-radius:10px;
}

button{
width:100%;
padding:12px;
margin-top:10px;
border:none;
border-radius:6px;
background:#81b64c;
color:white;
cursor:pointer;
font-size:16px;
}

.status{
margin:10px 0;
font-size:18px;
}

.clock{
background:#1f1d1b;
padding:10px;
border-radius:6px;
margin-bottom:10px;
font-size:18px;
text-align:center;
}

.moves{
background:#1f1d1b;
padding:10px;
border-radius:6px;
height:250px;
overflow:auto;
}

.highlight{
box-shadow: inset 0 0 3px 3px yellow;
}

</style>
</head>
<body>

<header>
<h1>♟ Play vs AI</h1>
</header>

<div class="container">

<div id="board"></div>

<div class="panel">

<div class="clock">
⚪ White: <span id="whiteClock">10:00</span>
</div>

<div class="clock">
⚫ Black: <span id="blackClock">10:00</span>
</div>

<div class="status" id="status">
White to move
</div>

<button onclick="newGame()">
New Game
</button>

<button onclick="board.flip()">
Flip Board
</button>

<h3>Moves</h3>

<div class="moves" id="moves"></div>

</div>

</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/chess.js/0.13.4/chess.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.js"></script>

<script>

const game = new Chess();

let whiteTime = 600;
let blackTime = 600;

let board = Chessboard('board', {

draggable:true,

position:'start',

pieceTheme:
'https://images.chesscomfiles.com/chess-themes/pieces/neo/150/{piece}.png',

onDragStart:onDragStart,
onDrop:onDrop,
onSnapEnd:() => board.position(game.fen())

});

function onDragStart(source,piece){

if(game.game_over())
return false;

if(game.turn()==='w' &&
piece.search(/^b/)!==-1)
return false;

if(game.turn()==='b')
return false;

}

function onDrop(source,target){

const move = game.move({

from:source,
to:target,
promotion:'q'

});

if(move===null)
return 'snapback';

updateStatus();
updateMoves();

setTimeout(aiMove,500);

}

function aiMove(){

if(game.game_over())
return;

const moves = game.moves();

const move =
moves[Math.floor(
Math.random()*moves.length
)];

game.move(move);

board.position(game.fen());

updateStatus();
updateMoves();

}

function updateStatus(){

let text='';

if(game.in_checkmate()){

text =
(game.turn()==='w')
?
'Black Wins!'
:
'White Wins!';

}
else if(game.in_draw()){

text='Draw';

}
else{

text=
(game.turn()==='w')
?
'White to move'
:
'Black thinking...';

if(game.in_check())
text += ' (Check)';

}

document
.getElementById('status')
.textContent=text;

}

function updateMoves(){

const history =
game.history();

let html='';

for(let i=0;i<history.length;i+=2){

html +=
(Math.floor(i/2)+1)
+'. '
+history[i];

if(history[i+1])
html+=' '+history[i+1];

html+='<br>';

}

document
.getElementById('moves')
.innerHTML=html;

}

function newGame(){

game.reset();

board.start();

updateStatus();

document
.getElementById('moves')
.innerHTML='';

}

function formatTime(seconds){

let m =
Math.floor(seconds/60);

let s =
seconds%60;

return m+':' +
String(s).padStart(2,'0');

}

setInterval(()=>{

if(game.game_over())
return;

if(game.turn()==='w')
whiteTime--;
else
blackTime--;

document
.getElementById('whiteClock')
.textContent =
formatTime(whiteTime);

document
.getElementById('blackClock')
.textContent =
formatTime(blackTime);

},1000);

updateStatus();

window.addEventListener(
'resize',
()=>board.resize()
);

</script>

</body>
</html>
