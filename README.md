# Python Automated Bulk WhatsApp Messages

This is a Python script that sends WhatsApp messages automatically using the WhatsApp web application with saved contact numbers. It can be configured to send advertising messages to customers. The script reads data from an Excel sheet and sends a configured message to each contact.

## Important
**WhatsApp Business API**: As of May 2024, WhatsApp Business released an API that can accomplish the same requirements as this repository. Consider using the WhatsApp Business APIs for more robust solutions.

## Prerequisites
Ensure your system has the following programs/packages installed. The contact numbers should be saved in your phone. While there is a way to send messages without saving the contact number, it has limitations for sending attachments.

* **Python 3.12**: Download it from [Python.org](https://www.python.org/downloads)
* **Selenium Web Driver**: Download it from [ChromeDriver](https://chromedriver.chromium.org/downloads)
* **Google Chrome**: Download it from [Google Chrome](https://www.google.com/chrome)
* **Pandas**: Run in command prompt `pip install pandas`
* **Xlrd**: Run in command prompt `pip install xlrd`
* **Selenium**: Run in command prompt `pip install selenium`

## Approach
1. **Log in**: User scans the web QR code to log in to the WhatsApp web application.
2. **Read Message**: The script reads a customized message from an Excel sheet.
3. **Search and Send**: The script reads rows one by one, searches for the contact number in the web search box, and if the contact number is found on WhatsApp, it sends the configured message. Otherwise, it reads the next row.
4. **Loop Execution**: The loop executes until all rows are processed.

**Note**: If you wish to send an image instead of text, you can add the attachment selection Python code.

## Legal
This code is not affiliated with, authorized, maintained, sponsored, or endorsed by WhatsApp or any of its affiliates or subsidiaries. This is an independent and unofficial software. Use at your own risk. Commercial use of this code/repo is strictly prohibited.

## Setup Instructions

### 1. Clone the Repository
```sh
git clone https://github.com/pythexcel/python-automation-bulk-whatsapp-message.git
cd python-automation-bulk-whatsapp-message
```

### Create virtual environment
```sh
python -m venv venv
```

# Activate virtual environment (Windows)
```sh
venv\Scripts\activate
```

# Activate virtual environment (MacOS/Linux)
```sh
source venv/bin/activate
```

# Install Requirements
```sh
pip install -r requirements.txt
```

# Run the Script
```sh
python script.py
```


By following these steps, you'll set up the environment, install the necessary packages, and run the script to send bulk WhatsApp messages automatically.


Example Excel Sheet
Your Excel sheet should have the following format:

| Contact Number  | Message               |
| -------------   | ----------------------          |
| 1234567890      | Hello, this is a test!  |

Make sure to customize your messages in the Excel sheet before running the script.
