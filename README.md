
🕷️ FunnelTrap

FunnelTrap is an advanced Python-based honeypot detector that performs behavioral, fingerprint, timing, and session-based analysis to determine the likelihood that a target system is a honeypot.

Designed to complement FunnelWS and work as a smart decoy trap scanner.

🚀 Features

🔍 Fingerprint & behavioral honeypot detection

🧠 Intelligent payload fuzzing and response timing analysis

🌐 Subdomain and port scanning with passive & active resolution

🧬 Session and entropy-based cookie inspection

🕵️ Block detection, fake URL analysis & Tor support for IP rotation

📊 JSON & HTML report generation

📦 Requirements

pip install -r requirements.txt

Or manually:

pip install requests beautifulsoup4 stem dnspython colorama

🛠️ Usage

# Clone the repository
git clone https://github.com/yourname/FunnelTrap.git

# Enter the project directory
cd FunnelTrap

# Run the honeypot detector
python3 main.py

The script will prompt for a target URL or IP and begin automated multi-phase scanning.

Generated reports:

report.json: Full structured result

report.html: Styled report with verdict & test details

🧪 Detection Methodology

FunnelTrap combines the following analysis techniques:

Technique

Description

Fingerprint

Header & content matching vs honeypot signatures

Behavioral

Fake URL, XSS/SQLi payloads & response time

Timing

Mean/stdev difference between various payloads

Session

Cookie consistency & entropy detection

Subdomain

crt.sh + DNS + open port checks

Block Detection

Admin/known paths + status code analysis

Similarity Check

Response content diffing between endpoints

🧅 Tor Integration (Optional)

FunnelTrap can use Tor to rotate IP addresses and bypass rate-limiting or detection mechanisms.

Make sure Tor is installed and configured correctly.

📄 License

MIT License

👤 Author

Developed by [Your Name or Handle]Inspired by modern active deception countermeasures and FunnelWS project.

📬 Contributions

Pull requests and improvements welcome!
Feel free to fork and adapt the honeypot signature set.

Stay hidden. Detect deception. ☠️
