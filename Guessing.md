```mermaid
    flowchart TD
    generate[Generate random number between 1 and 10] --> print_Q[Print: Guess number between 1 and 10]
    print_Q --> get_answer[Recieve player's answer]
    get_answer --> checkv[Check for valid answer]
    checkv --> valid[Answer is valid]
    valid --> check_answer[Check if player's answer = random number]
    checkv --> nvalid[Answer is invalid]
    nvalid --> try_again[Print: Please try again]
    try_again --> get_answer
    check_answer --> player_right[Player is right]
    player_right --> win((Player Wins))
    check_answer --> player_wrong[Player is wrong]
    player_wrong --> too_high[Answer is too high]
    too_high --> print_too_high[Print: Answer is too high]
    print_too_high --> get_answer
    player_wrong --> too_low[Answer is too low]
    too_low --> print_too_low[Print: Answer is too low]
    print_too_low --> get_answer
```
# Guessing Game Description:

The game starts by generating a random number between 1 and 10.  
The program then asks the player to choose a number between 1 and 10.  
The program then recieves the players answer.  
The answer is then checked to to see if it is valid (between 1 and 10 and numerical characters).  
If the answer is invalid, the program prints "Please try again" and the player is asked again.  
This repeats until the answer is valid.  
If the answer in valid, it is checked to see if it equals the random number.  
If the players answer is wrong, it is then checked to see if its too high or too low.  
If its to high, the program prints "Answer is too high" then loops back to the player inputing a new answer.  
If its to low, the program prints "Answer is too low" then loops back to the player inputing  a new answer.  
If the Player's answer equals the random number, the player wins.   



