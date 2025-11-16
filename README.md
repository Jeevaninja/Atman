⭐ ATMAN – Advanced Web Reconnaissance & Vulnerability Intelligence Framework

Atman is a powerful, modern, and highly configurable web reconnaissance framework designed for penetration testers, bug bounty hunters, and security teams.
It automates deep reconnaissance, vulnerability scanning, data intelligence, and continuous monitoring — giving you a complete picture of an application’s attack surface.

Atman correlates reconnaissance data using a database-backed architecture and offers intelligent GPT-powered insights, attack surface suggestions, and vulnerability descriptions.

🚀 What is Atman?

Atman is a next-generation web reconnaissance suite built to simplify and accelerate information gathering.
It combines:

Automated subdomain discovery

Port and service enumeration

Fuzzing & endpoint extraction

Vulnerability scanning

OSINT enrichment

Continuous monitoring

AI-driven recon intelligence

…and organizes everything into structured workspaces for teams, freelancers, and bug bounty hunters.

If you want a complete start-to-end recon pipeline, Atman gives you everything in one unified platform.

🧠 Key Capabilities
🔍 Deep Reconnaissance

Subdomain enumeration

Alive host detection

IP & open port identification

Directory & file fuzzing

Endpoint extraction

Screenshot capture

WHOIS & WAF detection

S3 bucket misconfiguration checks

Automated vulnerability scanning using:

Nuclei

Dalfox

CRLFuzzer

Additional recon and misconfiguration tools

📡 OSINT Intelligence

Employee enumeration

Email harvesting

Meta information gathering

Google dorking for exposed files/URLs

Related domain discovery

Related TLD mapping

🗂 Workspaces & Project Management

Organize recon data into separate, isolated workspaces such as:

Bug bounty programs

Client pentests

Internal audits

Long-term recon campaigns

Each workspace has its own dashboard and data store.

⚙️ Highly Configurable Scan Engines

YAML-based scan configurations

Customizable concurrency, rate limits, timeouts

Prebuilt engines (Full Scan, Passive Scan, OSINT Scan, Screenshot Scan)

Add your own recon pipelines

Support for parallel scans and subscans

Subscans allow you to run additional scans instantly on newly discovered assets — without waiting for the main pipeline to finish.

📑 PDF Reporting

Generate fully customized PDF reports such as:

Full Recon Report

Vulnerability Report

OSINT Report

Customize:

Themes & colors

Executive summary

Footer & branding

Company information

🤖 GPT-Powered Intelligence

Atman integrates GPT models to enhance recon quality:

🔎 Vulnerability Intelligence

Human-like descriptions

Impact analysis

Remediation guidance

Reference & context gathering

🛡 Attack Surface Suggestions

Based on:

Page titles

Open ports

Technologies

Subdomain patterns

Historical weaknesses

Atman recommends possible attack vectors with reasoning.

🔔 Continuous Monitoring

Schedule scans periodically or at exact times:

Every X minutes

Daily, weekly schedules

Clocked scans at specific HH:MM

Receive alerts for new:

Subdomains

Vulnerabilities

Recon changes

Supports notifications via:

Slack

Telegram

Discord

🧩 Advanced Recon Data Correlation

Using database-backed storage, Atman offers:

Smart duplicate removal

Recon data change detection

Autosuggestion-based filtering

Query language for recon filtering:

http_status=200&name=admin


Recon data visualization

Activity insights (most vulnerable assets, most common CVEs, etc.)

🧰 Toolbox

Atman ships with helpful built-in tools:

WHOIS lookup

CMS identification

CVE lookup

URL extraction utilities

Import/export of endpoints & subdomains

You can add custom tools or external GitHub/Go-based utilities.

👤 User Roles & Permissions

Teams can assign:

🔐 System Administrator

Full control over system configuration, scan engines, users, and tools.

🔍 Penetration Tester

Can create/edit targets, initiate scans, and manage recon — without editing system-level configs.

📊 Auditor

View-only access with ability to download reports.

🚀 Quick Installation (Ubuntu / VPS)
git clone https://github.com/jeevaninja/Atman
cd Atman

Configure environment:
nano .env


Update:

POSTGRES_PASSWORD

(Optional) Admin credentials for non-interactive install

Optional admin setup:
DJANGO_SUPERUSER_USERNAME=admin
DJANGO_SUPERUSER_EMAIL=admin@example.com
DJANGO_SUPERUSER_PASSWORD=yourStrongPassword

Run installation:
sudo ./install.sh


For non-interactive installation:

sudo ./install.sh -n


Access Atman at:

https://127.0.0.1


or your VPS public IP.

🛠 Updating Atman
cd Atman
sudo ./update.sh


If needed:

sudo chmod +x update.sh

📘 Contributing

Atman welcomes contributors!
You can improve:

UI/UX

Documentation

Features

Tool integrations

Recon engines

Bug fixes

Steps:

Fork the repository

Create a branch

Commit your changes

Submit a pull request

🛡 Reporting Security Issues

Please submit responsible disclosures via GitHub’s private vulnerability reporting system.


