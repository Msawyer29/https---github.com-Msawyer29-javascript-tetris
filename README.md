# javascript-tetris
A prototype model I designed for a school project using canvas to build a retro inspired version of Tetris.

Some of the current functions/features:
- Reset button
- Status: Playing / Game Over (when tetrominos reach top of gameboard)
- Controls A : move left, D : move right, S : move down, E : rotate
- Generate random tetrominos, all 7 classic shapes
- New shape falls at a speed of 1 line per second
- Wall, vertical and horizontal collision checks
- Check for completed rows, completion of a row = score +100 pts
- Completion of 4 rows (a "Tetris") = score +800 pts
- Move all shapes down based on the number of rows completed (and then deleted)

Improvements to make:
- Adjust game scale, my gameboard looks best at a scale of 2:2, however this requires user to zoom out of their browser to about 50% for best playing experience
- Add a pause button
- Display "next shape" on the right side of the gameboard 
- Implement game levels, every 10 lines completed, level increase +1, new shape falls faster, score calculator for level increase
- High score field, save high score in browser
- Add music/sfx
