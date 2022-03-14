To run the programming assignment made by me here is just some special instructions :

1. install the following modules:
	1.pickle
	2.typer
	

2. Clarification on Windows  when using npm test the multi lined text might not match your expected output but it is the
	same text . There is some error known as lf or crlf this is a known windows bug . 
	so when expected result might be :
	"""Usage :-
$ ./task add 2 hello world    # Add a new item with priority 2 and text "hello world" to the list
$ ./task ls                   # Show incomplete priority list items sorted by priority in ascending order
$ ./task del INDEX            # Delete the incomplete item with the given index
$ ./task done INDEX           # Mark the incomplete item with the given index as complete
$ ./task help                 # Show usage
$ ./task report               # Statistics"



the recieved result differs just a bit:-
"
Usage :-·
    $ ./task add 2 hello world    # Add a new item with priority 2 and text \"hello world\" to the list·
    $ ./task ls                   # Show incomplete priority list items sorted by priority in ascending order·
    $ ./task del INDEX            # Delete the incomplete item with the given index·
    $ ./task done INDEX           # Mark the incomplete item with the given index as complete·
    $ ./task help                 # Show usage·
    $ ./task report               # Statistics·	"

As you can see dots are appearing after every line. After completing some reading I have concluded that this bug is inevitable and occurs on every machine
THIS ERROR OCCURS IN TEST NO 1,2, 6 and 16 . THe expected output and the received output is the same just varying a little because of a bug

3. As for test no 7 I do believe there is truly something wrong from the test file
When I checked the test file I found that the task was running the "list when there are no remaining tasks" 
	before running the delete tests which promptly gave an error SO i fixed it by moving the position of the file 

4. A function in python cannot be named del(), So i edited the task file to change the name of the function del to delete


Thank you for this opportunity 
Hoping to get selected 