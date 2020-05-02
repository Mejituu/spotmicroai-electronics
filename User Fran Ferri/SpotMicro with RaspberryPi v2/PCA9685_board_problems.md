The generic PCA9685 board that you can buy everywhere has the following problems.

Problems:

* When you shut it down resets the controller in the board and the legs may jump to unpredictable positions, same efects when you re-enable the power in the board.

* The board takes 6v max for the servo power cirquit.

Solutions:

* You can feed any voltage you like if you power the servos directly in the very same servos connections in the board, the cirquit is isolated from the board one. Don't do this is you already have a board with a burned diode.
Mind than you are bypasing the capacitor this way. Is not ideal. But you can feed with any amount of voltage and amp that the board lanes can't take without affecting the board functions.

* If you go this path use a relay since you are bypasing the 0E conector

![PCA9685_bypass_connection](https://gitlab.com/custom_robots/spotmicroai/.png)

