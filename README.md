# Kenyatta National Hospital (KNH) Digital Infrastructure 

A secure shell scripting solution for managing and analyzing data from critical hospital sensors, including Heart Rate, Temperature, and Water Usage monitoring.

---

## Project Objective

This project aims to:

- Automate hospital environment setup using Shell Scripts.
- Secure sensitive medical logs through Linux permissions.
- Analyze critical sensor readings and generate reports.
- Archive logs with timestamps for record keeping.
---

## Project Overview

The system uses a Python-based data simulator (`hospital_system.py`) to generate sensor data.

Our shell scripts perform the following tasks:

- **hospital_admin.sh** → Creates directories and applies security permissions.
- **hospital_analysis.sh** → Detects critical patient readings and analyzes water usage.
- **hospital_archive.sh** → Archives logs and recreates fresh log files.
```

---

## Repository Structure

```text
Coding-lab_Group7/
├── hospital_admin.sh
├── hospital_analysis.sh
├── hospital_archive.sh
├── hospital_system.py
├── .gitignore
└── README.md
```

---

## System Setup

### Clone the Repository

```bash
git clone https://github.com/tmachingur-code/Coding_lab_Group7
cd Coding-lab_Group7
```

### Initialize Environment

```bash
./hospital_admin.sh
```

### Start the Data Engine

```bash
python3 hospital_system.py start
```

### Run Analysis

```bash
./hospital_analysis.sh
```

### Archive Logs

```bash
./hospital_archive.sh
```

### Stop the Data Engine

```bash
python3 hospital_system.py stop
```

## Technologies Used

- Bash Shell Scripting
- Linux File Permissions (chmod)
- grep
- awk
- Git & GitHub
- Python 3

