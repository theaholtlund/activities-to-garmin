# WIP: Garmin Connect and Intelligent Cycling

Project working with Garmin Connect data, potentially importang activities from Intelligent Cycling (if I can find a way to make it work lol, tricky one). Still need to implement:

- More elaborate secret management, use Azure? GitHub?

## Requirements

- Python ≥ 3.10, as this is required by GarminConnect
- ChromeDriver, which can be installed for example via Homebrew

## Create a Virtual Environment

```bash
python3.11 -m venv .venv
source .venv/bin/activate
```

## Install the Requirements

```bash
pip install -r requirements.txt
```

## Configure Environment Variables:

Create a .env file in the project root with the following content:

```bash
IC_USER="YOUR-IC-EMAIL"
IC_PASS="YOUR-IC-PASSWORD"
GARMIN_USER="YOUR-GC-EMAIL"
GARMIN_PASS="YOUR-GC-PASSWORD"
```

## Run the Project Files

Garmin Connect:

```bash
python garmin-connect.py
```

Intelligent Cycling:

```bash
python intelligent-cycling.py
```
