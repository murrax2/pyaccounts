=====
Login
=====

.. data:: loginui(#)

.. note:: The # in the brackets is not meant to be used, readthedocs won't let me do two brackets by themselves.
	
Use this when you don't have the user's details, it will prompt them to enter their details.
Raises a ValueError when login failed.

Example:
.. code-block:: python

	try:
		loginui()
		#Runs if they login correctly.
	except ValueError:
		#Runs if they fail to login.

.. data:: login(user, password)

Use this when you have the user's details.
Variables user and password are strings.
Raises a ValueError when incorrect details are passed.

Example:
.. code-block:: python
	
	user = input("What is your username?")
	password = input("What is your password?")
	try:
		login(user, password)
		print("Logged in")
		#Runs if they login correctly.
	except ValueError:
		print("Incorrect username or password")
		#Runs if they fail to login
		
.. toctree::
   :maxdepth: 2
   register.rst
  
   
