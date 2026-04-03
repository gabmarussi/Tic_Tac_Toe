# FECAP - Fundacao de Comercio Alvares Penteado

<p align="center">
<a href="https://www.fecap.br/"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRhZPrRa89Kma0ZZogxm0pi-tCn_TLKeHGVxywp-LXAFGR3B1DPouAJYHgKZGV0XTEf4AE&usqp=CAU" alt="FECAP - Fundacao de Comercio Alvares Penteado" border="0"></a>
</p>

# Tic-Tac-Toe

## Team Members:
Gabriel Marussi - RA: 24026609<br>
Arthur Rodrigues - RA: 24026567<br>
Vinicius dos Santos - RA: 24025961<br>
Matheus Rossaneze - RA: 24026354<br>
Pedro Schaurich Maia - RA: 24026011<br>
Lucas Oliveira da Silva - RA: 24025988

##
## Advisor Professor: <a href="https://www.linkedin.com/in/victorbarq">Victor Bruno Alexander Rosetti de Quiroz</a>

## Description:

This is a student project developed as a graded group assignment: a Tic-Tac-Toe game built in C# using Unity.
The game was designed to be simple, functional, and visually themed around a cyberpunk style.

It is a local single-player experience where the human player uses "X" and faces an AI opponent using "0". The AI prioritizes winning moves, then blocking moves, and uses fallback choices when needed, resulting in a very strong opponent that is difficult to beat.

### Features:

Some features were required by the assignment rubric and were implemented in this project:

* Local single-player game mode.
* Graphical interface with a menu scene.
* Strong AI behavior for turn decisions.

## Documentation

### Tech Stack

* Engine: Unity
* Language: C#
* UI: Unity UI (Text/Button-based board)

### Recommended Unity Version

To avoid compatibility issues, use Unity version <a href="https://unity.com/releases/editor/whats-new/2022.3.10">2022.3.10</a>.

### Project Structure

Main folders used in this repository:

* `Assets/Resource/Scripts/` - gameplay scripts (including game logic controller).
* `Scenes/` - playable scenes (`Menu.unity` and `Jogo.unity`).
* `ProjectSettings/` - Unity project configuration files.

### Core Gameplay Flow

1. The player starts from the menu scene.
2. A game scene opens with a 3x3 board.
3. The player places an "X" on an available tile.
4. The AI immediately responds with "0" based on priority logic:
	* Complete a winning line if possible.
	* Block the player's immediate winning line.
	* Prefer central tile when available.
	* Use fallback/randomized valid positions.
5. The game checks for win or draw outcomes.

### How to Run

1. Install Unity Hub and Unity Editor 2022.3.10.
2. Clone or download this repository.
3. Open the project folder in Unity Hub.
4. Open a scene from `Scenes/`:
	* `Menu.unity` (entry point), or
	* `Jogo.unity` (direct gameplay).
5. Press Play in the Unity Editor.

### Notes and Limitations

* The game currently targets local play only.
* There is no match history or score persistence between rounds.
* The implementation is focused on assignment goals and gameplay behavior.

### Possible Future Improvements

* Add score tracking and persistent statistics.
* Improve AI architecture for maintainability and testability.
* Add sound effects, animations, and additional UI feedback.
* Add difficulty levels (easy/normal/hard).

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
