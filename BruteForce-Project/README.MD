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

