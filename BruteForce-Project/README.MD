Brute Force Attack & Defense Project:-
This Python project demonstrates how brute force attacks work and how to defend against them using rate limiting and account lockouts. Made for cybersecurity learning only.

Requirements:-
- Python 3.x
- Flask
- requests

Installation:-

Install Flask:
pip install flask

Install requests:
pip install requests

Project Structure:-
defensive-tool/    - Rate limiting and account lockout defense server
offensive-tool/    - Brute force attack simulation script
screenshots/       - Project demonstration and testing results

How to run:-
Step 1: Start Defense Server (Run this first)

cd defensive-tool
python test_server.py

Server will start at: http://127.0.0.1:5001/

Step 2: Run Attack Tool (Open new terminal)
cd offensive-tool
python brute_force.py

Watch the attack attempts and see how defense blocks repeated failed logins!

Defensive Tool - How It Works:-
Tracks failed login attempts per user and IP address
Blocks account after 3 failed password attempts
Applies 60-second lockout period
Returns HTTP 429 (Too Many Requests) status code
Displays lockout message to users

Offensive Tool - How It Works:-
Tests multiple password combinations automatically
Sends POST requests to login endpoint
Logs success/failure for each attempt
Stops when correct password is found
Demonstrates brute force attack mechanism

HTTP Status Codes Used:-
200 (OK) - Successful login with correct credentials
401 (Unauthorized) - Login failed due to wrong username or password
429 (Too Many Requests) - Account locked after excessive failed attempts, rate limiting active

Screenshots:-
Project demonstration available in /screenshots folder showing complete attack-defense lifecycle.

What I Learned:-
- Brute force attack mechanisms and automation
- Rate limiting and temporary IP blocking techniques
- Flask web application security implementation
- HTTP status codes for security responses (200, 401, 429)
- Offensive and defensive security concepts
- Real-time threat detection and response systems
- Account lockout mechanisms to prevent unauthorized access


Disclaimer:-

For educational use only—never run on systems without permission.

