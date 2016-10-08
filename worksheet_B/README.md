INPUT random 5 letter word from given list i.e."Sheep", "Towel", "Light", "Learn", "Third", "Every"

DECLARE word variable

DECLARE correctanswer variable

DECLARE guesscount variable

SET correctanswer to False

SET guesscount to 0

WHILE guesscount is less than 4

    DISPLAY 'You have a 5 letter word'

    DISPLAY 'Can you guess what it is? Enter here:'

	  User INPUT guess

	  DECLARE guess variable

	  IF guess is equal to 5
		    ARRAY word variable, DECLARE as 'wordlist'
		    ARRAY guess variable, DECLARE as 'guesslist'
		    SET matching to 0

        FOR i in range(0, 5):
		  IF guesslist [i] is the same as wordlist [i]:
			SET matching to matching + 1
		IF matching is 0
			DISPLAY 'Score: 0/5'
			SET guesscount to guesscount + 1
		IF matching is 1
			DISPLAY 'Score: 1/5'
			SET guesscount to guesscount + 1
		IF matching is 2
			DISPLAY 'Score: 2/5'
			SET guesscount to guesscount + 1
		IF matching is 3
			DISPLAY 'Score: 3/5'
			SET guesscount to guesscount + 1
		IF matching is 4
			DISPLAY 'Score: 4/5'
			SET guesscount to guesscount + 1
		IF matching is 5
			DISPLAY 'Correct!'
			SET correctanswer to True
			SET guesscount to 4

    ELSE, DISPLAY 'You need to guess a FIVE letter word'
	END WHILE

IF correctanswer is False
	DISPLAY '4 incorrect entries, Game Over"

ELSE
	DISPLAY 'Well done!
	
https://cloud.githubusercontent.com/assets/22060783/19214237/694f8968-8d76-11e6-998b-c2ede6d8c387.png	
