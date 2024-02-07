# Gomoku AI
Gomoku AI.

## Description
This project utilizes minimax and alpha-beta pruning algorithms to implement a Gomoku AI.

## Getting Started
### Dependencies
- Linux

### Packages
- baselines - Provide baselines based on simple algorithms.
    - baseline1 - pure random
    - baseline2 - minimax with simple value function

- src - Where you compile and run the program.
    - alphabeta.cpp - the AI based on alpha-beta pruning
    - main.cpp - game runner
    - makefile - compile the code
    - minimax.cpp - the AI based on minimax
    - playerRandom.cpp - the pure random AI

### Installing
```bash
git clone 
```

### Executing Program
1. Go to the "src" folder.
    ```bash
    cd src
    ```
2. Compile al programs.
    ```bash
    make
    ```
3. Start the game. \<AI1> and \<AI2> are the AIs to compete against each other.
    ```bash
    ./main ./<AI1> ./<AI2>
    ```
    Here are some examples:
    ```bash
    ./main ./alphabeta ./minimax
    ./main ./alphabeta ../baselines/baseline2
    ```
4. After the game finishes, it will generate a file named "gamelog.txt" in the "src" folder.

### Help 
- Clean the executables under the "src" folder.
    ```bash
    make clean
    ```
- If you encounter the following error when you run the game, 
    ```bash
    timeout: failed to run command ‘../baselines/baseline1’: Permission denied
    ```
    use the "chmod" command to add executable permissions.
    ```bash
    chmod +x ../baselines/baseline1
    ```