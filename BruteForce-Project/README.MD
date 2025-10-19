Brute Force Attack & Defense Project:-

This Python project demonstrates how brute force attacks work and how to defend against them using rate limiting and account lockouts. Made for cybersecurity learning only.

Requirements:-
- Python 3.x
- Flask
- requests

Defensive Tool — Rate Limiter & Account Lockout

This is a simple Python Flask server that protects a login page from brute force attacks.

What It Does:
Tracks failed login attempts for each user or IP address.
If someone enters the wrong password 3 times, their account is locked for 1 minute.
Shows a lockout message on the web page and sends a special error code (429) for scripts.

How to Use:
Open a terminal in this folder.
Install Flask: pip install flask
Run the server:
Open http://127.0.0.1:5001/ in your browser.
Try logging in with wrong passwords to see the lockout in action.

How to run:-
cd defensive-tool
python test_server.py

Open browser at: http://127.0.0.1:5001/


Offensive Tool — Brute Force Attacker:
This is a simple Python script that performs a brute force attack on a test server's login page.  
It tries a list of passwords one by one until it finds the correct password.

How to Use:
1. Make sure the test server (defensive tool) is running.
2. Open a terminal in this folder.
3. Install the required library:
pip install requests
4. Run the script:
python brute_force.py

What This Script Does:
- Sends login requests to the server using different passwords.
- Stops when the correct password is found.
- Shows the result in the terminal.

Run Attack Tool (Optional):
cd offensive-tool
python brute_force.py

What I Learned:-
- Brute force attack mechanisms
- Rate limiting and temporary IP blocking
- Flask web application security
- Offensive and defensive security concepts

Disclaimer:-
For educational use only—never run on systems without permission.


