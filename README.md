# javascript-tetris
A prototype model I designed for a school project using canvas to build a retro inspired version of Tetris.

Some of the current functions/features:
- Reset button
- Status Display: Playing / Game Over (when tetrominos reach top of gameboard)
- Controls A : move left, D : move right, S : move down, E : rotate
- Generate random tetrominos, all 7 classic shapes
- New shape falls at a speed of 1 line per second
- Wall, vertical and horizontal collision checks
- Check for completed rows, completion of a row = score +100 pts
- Completion of 4 rows (a "Tetris") = score +800 pts
- Move all shapes down based on the number of rows completed (and then deleted)

Improvements to make:
- Debug: On the initial page load from the https://msawyer29.github.io/javascript-tetris-demo/ link, the gameboard font does not load until the user clicks the "Reset" button or refreshes the browser window. I have tried different approaches to ensure the "Press Start 2P" font loads successfully when displaying the gameboard for the first time. Currently after the font is loaded I have the rest of the canvas drawing functions being called:

font.load().then( () => {
        // Call the rest of the canvas drawing functions after the font is loaded
        drawCanvas();
    });
    
But this only works when loading the gameboard from Visual Studio Code. Still working on a solution.
- Adjust game scale: with my current canvas design my gameboard looks best at a scale of 2:2, however this requires user to zoom out of their browser to about 50% for the best playing experience with the gameboard centerscreen in the browser. When my canvas ratio is set at 1:1, the gameboard does not center properly on most browser windows....working on it
- Add a pause button
- Add "Next Shape" Display on the right side of the gameboard, make "Status" Display smaller
- Implement game levels, every 10 lines completed, level increase +1, new shape falls faster, score calculator for level increase
- High score field, save high score in browser
- Add music/sfx
