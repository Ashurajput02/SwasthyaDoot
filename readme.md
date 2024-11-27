1.here in this project my role was specific to write the extensive backend code for the admin panel as well as merge the frontend part of the code with the backend code .
2.It is a simple website idea which allows you to book virtual /physical appointments at just one click with best doctors in the world and that too at the ease of your house . All you need is to just go to the website , create an account , choose a doctor , choose a particular time and do the necessary payment and you are done .

3.in this project ---
the backend stuff--
so we have 3 basic functionalities ---

BASIC ER MODEL --
a---appointments to be done (m:n  cardinality)
b---- doctors can register (DOCTOR)
c---- user can register(USER)


so thats why created 3 models
--userModel.js
--doctorModel.js
--appointmentModel.js


4.separate routes to all the possible pages are present in the routes section 
5. now as the users type in our codebase ---admin, doctor, naive user
so need different types of auth access for all of them as each has different set of permissions some of which are common to all and some are exclusive to only one set of users, so created different auth access for each as well as different routes for different users.

6. Talking about the security :
a. in this version of the project  , jwt token based authentication is there but otp authentication is not available currently due to google mail policies. 
b.however,in the previous internship expereince i have implement otp authentication via nodemailer as well .Due to ongoing exams , unable to make changes in this project.
c.the codebase efficiently ensures that an unauthorized user is not able to access the routes which are specific to roles,
like without admin login a normal user cant access exclusive admin pages 
d.this codebase make use of mongo db  as the database , however can be easily shifted to relational database as well .
e. the code is made highly scalable and efficient code writing practices are used to ensure that it is easy to modify and let others grasp the code
f.users can also log out easily.
