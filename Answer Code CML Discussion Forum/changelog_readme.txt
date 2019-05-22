----------------------------Change Log:------------------------------

Note: All new comments added are in Block Letters for easy identification
---------------------------------------------------------------------

1.	Completed the following parts of the project:
		•Question.java
		All of the constructors and methods in this class

	•Reply.java
		All of the constructors and methods in this class

	•The following methods in AbstractEntity.java
		getId
		setId
		autoGenerateId

	•The following methods in UserActivity.java
		postNewQuestion
		seeAllQuestions
		deleteQuestion
	•The following method in UpvoteServiceImpl.java
		getUpvote
---------------------------------------------------------------------
2.	Handled NumberFormatException, so if the user enters a string as inputFromUser instead of number the code does not crash.

 	Changes made in DiscussionForum.java to following methods of class DiscussionForum:
		menu(User, UserActivity)
		roleFromMenu()
		questionMenu(UserActivity, User)
		replyMenu(UserActivity, User, Question)
	And in UserActivity.java for the following methods of class UserActivity
		getQuestion()
---------------------------------------------------------------------
3.	Added an option to ‘Logout and Exit’ the program from main menu

	Changes made in DiscussionForum.java to following methods of class DiscussionForum
		main()
		menu(User, UserActivity
---------------------------------------------------------------------
4.	Corrected the code so a standard user cannot Upvote his own question/Answer(Allowed for Admin/Moderators).

 	Changes made in UpvoteServicesImpl.java to following methods of class UpvoteServicesImpl:
		addUpvote(Reply, User)
		addUpvote(Question, User)
---------------------------------------------------------------------
5. 	If a question was deleted, the code was not updating the ID of the 
	following questions after that.
	For example:
	1. Question Title - write
	Question - how to write
	2. Question Title - read
	Question - how to read
	3. Question Title - remember
	Question Title - how to remember
	
	If I deleted the 2nd Question and printed all the questions again it would show
	1. Question Title - write
	Question - how to write
	3. Question Title - remember
	Question Title - how to remember

	Changes made in QuestionServiceImpl.java to following methods of class
	QuestionServiceImpl:
		deleteQuestion(Question)
---------------------------------------------------------------------
