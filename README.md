chess-tutorial-site/

index.html
css/
 └─ style.css
js/
 ├─ app.js
 ├─ lessons.js
 ├─ puzzles.js
 └─ board.js
data/
 ├─ lessons.json
 └─ puzzles.json
 [
  {
    "title":"Mate in 1",
    "fen":"6k1/5Q2/6K1/8/8/8/8/8 w - - 0 1",
    "solution":"Qg7#",
    "hint":"Look for a queen move."
  }
]function puzzleSolved() {
  alert("🎉 Puzzle Solved!");
}<div id="winModal" class="modal">
  <h2>🎉 Puzzle Solved!</h2>
  <button onclick="closeModal()">Continue</button>
</div><iframe
width="100%"
height="315"
src="https://www.youtube.com/embed/OCSbzArwB10"
allowfullscreen>
</iframe>
function fullscreenBoard() {
  document.documentElement.requestFullscreen();
}<button onclick="fullscreenBoard()">
Fullscreen
</button>
localStorage.setItem(
  "lessonsCompleted",
  completedCount
);Progress: 8 / 16 Lessons
Puzzles Solved: 22
const dailyPuzzle =
puzzles[
  new Date().getDate() %
  puzzles.length
];
