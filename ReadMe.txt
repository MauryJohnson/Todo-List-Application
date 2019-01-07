ToDo List by Maury Johnson

1. Installation/Execution 			
	a. Install Java JDK 10 or later from this website: https://www.oracle.com/technetwork/java/javase/downloads/index.html
	b. Make sure that Java is configured correctly. Use this website to confirm your Java version: https://www.java.com/en/download/installed.jsp?detect=jre
	c. Double click ToDoList.jar file to run program.
	d. IF THERE are any problems executing the jar file, use this website: https://bitstorm.org/jarx/ (Supported by Windows 98 and up)
	   and use the program to execute the jar file.
	   
2. Login
	a. Able to create, delete, or log into a user with or without a password.
	b. Have the option to show password or not.
	
3. ToDo List
	a. This is where you can add and delete todo's.
	b. Quick adding feature allowed.
		i. For example, when adding a todo, can add a todo and all tasks using Add TODO button in the format: ToDo_Name1,Task_Name1,Task_Name2,Task_Name3.
		ii. When a ToDo is selected, can add one or multiple tasks using Add Task button in the format: Task_Name1,Task_Name2,Task_Name3.
		iii. No duplicate ToDo names or Task Names within a ToDo are allowed.
		iv. View TODO will allow user to view all tasks of ToDo selected and add, delete, or view task.
		v. Set Alert button will allow you to view all tasks of ToDo selected and set an alert to be used to notify user of a task to be done for a specific ToDo.
		vi. TODO Search button allows you to search for all tasks of a specific ToDo that have a date and time.

4. Set Alert
	a. To set an alert, find Set Alert button at first window after login and click it.
	b. You will see a list of all tasks for the ToDo. You can confirm or delete a due date for these tasks. ****THIS WILL EFFECT YOUR ALERTS IN REAL TIME****	
	c. if you enter only a date, time will be set to the minimum time. If you enter only a time, date will be set to current day. These are the cases, because when the program checks each task date times to alert user, it will compare current date time to these date times, which make the most sense for alerts.
	d. EasyTime button is a toggle button which allows conversion between 0-24 hour time to 12AM-12PM time. This also allows user to enter in 12AM-12PM time, for example:
	With EasyTime toggle button off, user can enter 00:03:29.
	With EasyTime toggle button on, user can enter 12:03:29AM.
	The program will remember this information as long as ToDo List SaveFolder is kept.

5. Set Notification
	a. For those who want even more flexibility with their alerts, find Set Notification Button on bottom right of Set Alert Window.
	b. You will be able to add or delete a notification date before due date in two formats:
		i. The first format will be with Notify Before Due Date toggle button off. You will enter a date, time, or both. The date and time entries will be handled the same way they were for Set Alert, and you will be alerted of the task at the added date and time.
		ii. The second format will require Notify Before Due Date toggle button to be on. You will enter a time in the text field to the right. This time will correspond to the amount f hours, minutes, and seconds to be notified before the due date. For example:
	1:22:00 will set up a notification that is 1 hour, 22 minutes, and 0 seconds before the due date time.
		iii. Deletion of a notification only requires the notification to be selected and the Delete Notification button to be clicked.
	c. You can also add multiple notifications usinng AddUntil and DeleteUntil buttons.
		i. AddUntil requires either a Date which is after current date and a time, or a time which is after current time and a date.
		ii. This will then add all notifications for each current date/time until the date/time after.
		iii. Useful if you want a lot of times/date notifications which are spaced apart evenly.
		iv. You can change how long you want to space apart each date/time by appending to your date/time Y, 
		indicating by year for date, M, indicating by month for date, D, indicating by day for date, h, 
		indicating by hour for time, m, indicating by minute for time, and s, indicating by second for time.
		The default configurations will be for day and minute.
		v. DeleteUntil works the same way.
		vi. After entering Y,M,D,h,m,s, you don't have to enter it again for every AddUntil/DeleteUntil.
		vii. Example input 1: DATE:1/10/2019Y TIME:6:00AM
		     Example input 2: DATE:1/1/2019  TIME:11:59PMm
			 Example input 3: DATE:1/3/2019D TIME:22:00:00s -> 
			 1. If date matches current day and time is greater than current time, it will create time 
			 	increments for that day until it reaches given time.
			 2. If date is greater than current day, it will create date notifications with the same time 
				for each date incremented until it reaches given date.
			  
6. ToDo List Alerts Popup
	a. If a task reaches its notification deadline, a ToDo List alert will popup, showing every ToDo followed by their tasks that reached its notification deadline.
	b. THIS REFRESHES IN REAL TIME, so you can either ignore this by pressing the Toggle Sound toggle button to turn off the sound, or press Acknowledge All button to acknowledge all tasks that reached their deadlines for their notifications/due dates.
	c. Acknowlege button will allow user to choose a task from a ToDo list to acknowledge. The user can acknowledge a task's due date or the notification.
	d. As long as user is logged in, all new due dates/notifications will be added to the User Alerts, so it is recommended for the user to keep the sound on.

7. ToDo Search
	a. Quickly gather all of your tasks given a range of dates and times.
	b. Can set each found tasks to a random date and time given by your next date and time input.

7. Extras
	a. Can use tab to transition between buttons and lists.
	b. Can also use arrow keys to traverse a list of items. This may be useful when given many tasks in a ToDo.
	c. Set Notification automatically detects EasyTime input or otherwise.