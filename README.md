A lightweight yet powerful Python script designed to perform an automated security audit and vulnerability assessment on WordPress websites. It checks for basic security configurations, exposed files, active plugins/themes, exposed usernames, and server infrastructure details.

🚀 Features
Infrastructure & Hosting Check: Automatically resolves the target IP address and looks up the ISP/Hosting provider and country.

Security Headers Analysis: Checks for essential HTTP security headers (HSTS, X-Frame-Options, X-Content-Type-Options, CSP, etc.).

Version Disclosure Check: Detects if the WordPress version is exposed via meta tags.

User Enumeration: Scans the WordPress REST API to check if author/user slugs are publicly exposed.

Plugin & Theme Detection: Extracts and lists detected plugins and themes from the website source code.

Database & Debug Check: Checks for exposed debug logs or database indicators.

Color-Coded Output: Highlights critical risks, usernames, and versions in clear colors (using colorama) for instant readability.

📋 Prerequisites
Make sure you have Python 3 installed on your system. You will also need the following Python libraries:

Bash
pip install requests beautifulsoup4 colorama
⚙️ Installation & Usage
Clone or download this repository:

Bash
git clone https://github.com/YOUR-USERNAME/wp-sicherheits-checker.git
cd wp-sicherheits-checker
Run the script:

Bash
python wordpress_pentest.py
Enter the target URL when prompted (e.g., example.com or [https://example.com](https://example.com)).
