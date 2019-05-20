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