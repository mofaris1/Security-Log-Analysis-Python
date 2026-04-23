# Security Log Analysis & Threat Detection

## Overview
This project focuses on applying data science techniques to analyze real-world security logs. Using Python and Pandas, the project parses, analyzes, and visualizes unstructured log data from different sources to identify patterns and assess potential security threats. 

## Datasets Analyzed
1. **Apache Web Server Logs:** ~56,481 entries.
2. **Firewall Logs:** Network connection logs.
3. **SSH Authentication Logs:** Focused on failed SSH login attempts.

## Key Objectives & Tasks
- **Log Parsing:** Utilized Regular Expressions (Regex) to extract structured data from raw log files.
- **Threat Assessment:** Analyzed HTTP status codes (e.g., 403, 404) and SSH login failures to identify brute-force or reconnaissance attacks.
- **Cross-Dataset Correlation:** Tracked common suspicious IP addresses across both SSH and Apache logs to build a timeline of events.

## Key Findings
During the cross-dataset correlation analysis, a specific IP address was identified performing a reconnaissance pattern: a single failed web request followed by two failed SSH login attempts. 
**Recommended Action:** Basic monitoring and rate-limiting login attempts for SSH, as well as hiding server banners on Apache.

## Technologies Used
- Python
- Pandas & NumPy
- Matplotlib & Seaborn (for data visualization)
- Regular Expressions (Regex)

## Team
- Yahia Abulibdeh 
- Mohammad Faris
