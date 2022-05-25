# 449-project-2

Team members

Akshaya RK
Priyansha Singh
Robin Khiv


Description:

A public Json API for Wordle. 

The project was inspired by the game Wordle and built as a REST API. This implementation of Wordle in Python is meant to be played as a REST API. Each game instance will have a secret word that each user can try to guess. The length of each word is currently set to 5 letters long. Players are allowed only 6 attempts at each word per game. Each guess must be a word from the english dictionary and 5 letters long. After guessing each word, the player will receive some output pertaining to the guess and all the guesses made. If the letter in the guess is in the correct position as the letter in the secret word, then it will be denoted with the word green. If the letter is in the word but not at the correct position then the letter will be denoted with the word yellow by the letter. if the letter does not exist in the word then the letter will be denoted with the word gray. 

Steps to start the databases and APIs:

1.Go inside 449proj/fastapi folder

2.Run the following command to initialize the databases(words,answers)
    ./bin/init.sh

Note:if permission denied error comes when running init.sh file then give permissions to file by going inside bin folder and running below command
 chmod 777 init.sh
 then come out of bin folder and run command 2 again
 
3.Run the following command to start both APIs(validate and compare)
    foreman start

4.Test the API calls using below urls
validate-http://localhost:5000/docs
compare-http://localhost:8000/docs