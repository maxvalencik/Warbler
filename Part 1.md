#Part One: Step Seven

- **How is the logged in user being kept track of?**

	By adding the user.id to the Session using the do_login(user) function defined in app.py


- **What is Flask’s g object?**

	The g object in flask is a global space where data can be stored during a single app context.
	
	
- **What is the purpose of add_user_to_g?**

	Adding the current user stored in the session to the g object. The g object is cleared after between each request so the function needs to be called before each of them.

- **What does @app.before_request mean?**

	It allows to execute the function listed (here add_user_to_g) before each request.