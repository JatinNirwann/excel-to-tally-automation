# Excel to Tally Automation Script

This Python script automates the process of transferring data from an Excel file into Tally or similar accounting software. It uses pandas to read Excel data and pyautogui to simulate keyboard inputs, making data entry quick and efficient.

## Features

- Reads data from an Excel file
- Simulates keyboard inputs to enter data into Tally
- Handles various date formats
- Includes configurable delays to accommodate different system speeds

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.6 or higher installed on your system
- pip (Python package installer)

## Installation

1. Clone this repository to your local machine:
   ```
   git clone https://github.com/your-username/excel-to-tally-automation.git
   ```

2. Navigate to the project directory:
   ```
   cd excel-to-tally-automation
   ```

3. Install the required Python packages:
   ```
   pip install pandas pyautogui
   ```

## Usage

1. Place your Excel file in a known location on your computer.

2. Open the `excel_to_tally_automation.py` file and update the `excel_path` variable with the path to your Excel file:
   ```python
   excel_path = r"path/to/your/excel_file.xlsx"
   ```

3. Run the script:
   ```
   python excel_to_tally_automation.ipynb
   ```

4. You will have 10 seconds to switch to your Tally software (or the application where you want to input the data).

5. The script will automatically start entering data. Ensure your Tally is ready to receive inputs in the correct fields.

## Customization

- You can adjust the sleep times in the script to match the speed of your system and Tally's responsiveness.
- Modify the column names in the script if they differ from your Excel file's structure.

## Troubleshooting

- If the script is moving too fast or slow, adjust the `time.sleep()` values.
- Ensure your Excel file has the correct column names: "Company Name", "GSTIN No.", "Amount", and "Date".
- If you encounter date formatting issues, check the `try-except` block in the script and adjust as needed.

## Contributing

Contributions to this project are welcome. Please feel free to submit a Pull Request.


## Disclaimer

-This script simulates keyboard inputs. Use it responsibly and ensure you have permission to automate data entry in your organization. Always verify the entered data for accuracy.
-It is recommended to test on a dummy data first to ensure its working properly as required.
-Also don't change windows or tab because it will interept data entry and fixing it will be very painfull. 