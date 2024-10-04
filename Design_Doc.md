This program acts as a digital magic 8-ball that gives you a randomly
generated answer every time you ask a question and "shake" it. The program creates a
text file and populates it with possible replies from the 8-ball, then picks and displays
a random reply to answer the user's question. This whole iteration continues until the
user enters "q" signaling that they got bored with the 8-ball.

---

Logical Steps:  

1. Create document for populating with 8-ball answers.
2. Write answers into the document.
3. Read the answers and store them in an empty list.
4. Use random.choice method on the list and save it to a variable.
5. Prompt user to type a yes/no question.
6. Display the randomized choice variable as the 8-ball's answer to the user's question.
7. Prompt user to choose whether to continue questioning the 8-ball or quit.
8. Reiterate the loop until the user decides to quit.

---

Variables: 
 
1. DIVIDER: Small detail that makes output more legible.
2. answers: Referenced for opening, closing, and writing in the 8ball_responses.txt file.
3. data: For accessing the txt file's contents.
4. options: Empty list that gets filled with "data".
5. answer: A randomized choice from "options" that serves as the answer to
	the user's question.
6. again: User input that determines whether the loop reiterates or ends.

---

Functions:
1. Function Name: magic8ball 
   Description: Main function that contains "the game flow" (every other function).
   Parameters: none 
   Returns: none

2. Function Name: generate_answer 
   Description: 1st function to execute in magic8ball(). Creates a txt doc with magic 8-ball answers, 
	stores each answer into a list, generates a random answer and saves it to "answer". 
   Parameters: none  
   Returns: none

3. Function Name: q_and_a  
   Description: 2nd function to execute in magic8ball() where the user asks a question and receives a 
	randomized answer from "options".
   Parameters: answer 
   Returns: none

4. Function Name: replay_or_end 
   Description: 3rd (last) function to execute in magic8ball(). Conditional statement determines 
	if magic8ball() loop will reiterate or end.
   Parameters: none
   Returns: none
