# Flow
The flow which i assumed is like this:-
1.user will login and then he will see list of exams which he want to practice.(these apis will be called from frontend)
2.after selecting exam he will see list of section which he wants to practice.
3. when he will select section he will see list of topics he want to practice.
4.after selecting topic he will see list of quizzes available for that particular topic.
5.then he will select quiz which he wants to practice and there he will see all the questions releated to that quiz.
6. whenever user will answer a question we will save it in Answer table with user_id,question_id and option_id
so that if if there is network peoblem or anything next time he can start from that question dont need to reanswer all previous question 
and while fetching we can fetch those questuons from answer table(this same functionallity can be used to show question 
second time when he will navigate to quiz after solving)
Didnt have time to implement this answer api justt model i have created(wasted maximum time in that signal thing, that was giving some error)
## API Documentation

The Quiz app have following api's:

#user apis

1./users/users/login  --for login user
2/users/users/logout   --for logout user
(here forgot to create register api)

#exam apis
1. /exams/  ---this api will send list of all exams
2. /exam/{exam_id}/sections  --this will send all the sections for a particular exam
3. /section/{section_id}/topics   -- this will send all the topics for a particular section
4. /topic/{toipc_id}/quizzes   --this will send all the quizzes for that particular topic
5. /quiz/{quiz_id}/questions   -- this will send all the questions for a particular quiz with options
