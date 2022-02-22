# Quiz_game
A quiz game where questions are true/false or yes/no and two players compete, gaining a point for a correct answer and losing a point for a wrong answer

Design Details

There are 7 true/false questions and the sequence of questions is determined by a random number generator and using linear probing on the list of questions. 
A random number between 1 and 6 is generated and used as a step length. The question sequence will be determined by stepping forward through the list of questions by
the step length, skipping over questions that have already been asked, wrapping around once the question number has passed 7, and ending the game one all 7 questions have been answered.
This linear probing inspired method works because 7 is a prime number so this algorithim is guranteed to ask all questions.

Made with an AMTEL AT89LP51IC2 microcontroller and programmed in 8051 assembly.
A BO230XS serial USB Adaptor is used to interface with a laptop to upload code onto the microcontroller  
An LCD 1602 module is used to display questions and points  
A 22.1184MHZ crystal is used for the clock.  
Four homemade capacitive sensors made with cardboard and aluminum foil are used as buttons triggered by a human hand and not pressure  
Four Texas Instruments NE555P timer chips are used in the astable osscilaor configuration, and the output frequency is used to determine capacatince
Wires are twisted and timers are spaced apart to minimize noise
Buzzer tones are used to signal wins and losses 
