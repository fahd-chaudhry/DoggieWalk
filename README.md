# DoggieWalk
## This repository features the DoggieWalk Web Application using Python, Flask, PostgreSQL, Nginx, and provisioned using Vagrant and Chef.

## To start the application, enter the commands below in bash terminal or equivalent:
- `vagrant up` <p>
- `vagrant provision` (Only needed if you have run vagrant up before and made changes) <p>
- `vagrant ssh` <p>
- `cd project` <p>
- `run **gunicorn --bind 0.0.0.0:5002 wsgi**` <p>

### Common Error:
Error: `Cannot connect to port 5002, port already in use` <p>
Solution: `run **fuser -k 5002/tcp > /dev/null 2>&1; exit 0**` <p>


### Technologies used:
- **Gunicorn** ‘Green Unicorn’ is a Python WSGI HTTP Server for UNIX. <p>
- **Nginx** is an HTTP and reverse proxy server.
- **Vagrant**
- **Python**
- **Flask** 

#### Sample user credentials:
- Email: `user1@sfu.ca`
- Password: `123456`

#### Addtional functions:
- Users get email notifications when they register as a new user and when they receive messages from other users. <p>
- Users get an inbox message when they receive a review
- The search bar can search:
	- users by name, email and city
	- search events by name, user and city
	- search dogs by breed
- Users can give other users reviews but not themselves

#### The url we use:
- `0.0.0.0:5002`

Main code is in: doggiewalk.py <p>
Feel free to modularize the code. <p>

### Contact Information:
- Fahd Chaudhry: `fahd.chaudhry@yahoo.com`
