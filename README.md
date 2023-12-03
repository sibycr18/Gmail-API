# Gmail API Email Management

This script utilizes the Gmail API to perform various email management tasks, such as fetching emails, applying labels, and creating new labels. It is designed to run as a standalone application and provides a convenient way to interact with Gmail programmatically.

## Prerequisites

Before running the script, ensure you have the required dependencies installed within a virtual environment:

1. **Create a Virtual Environment:**

   ```bash
   python -m venv venv
   ```
2. **Activate the Virtual Environment:**
	```bash
   # On Windows, use 
   venv\Scripts\activate
   # On Linux/mac, use
   source venv/bin/activate
   ```
3. **Install Dependencies:**
	```bash
	pip install -r requirements.txt
	```

## Setup 
1. **Enable Gmail API:**  
- Visit the [Google Cloud Console](https://console.cloud.google.com/) .
- Create a new project or select an existing one.
- Enable the Gmail API for your project. 
- Download the credentials JSON file and save it as `credentials.json` in the same directory as the script. 
2. **Authentication:**  
- Run the script, and it will guide you through the OAuth flow to authenticate and authorize the application. The authentication token will be saved as `token.json`.

## Usage 
1. **List Labels:**
   The script will list the available user defined labels in your Gmail account. 
2. **Fetch Emails:**
   Specify the number of emails to fetch, and the script will display the message IDs along with sender details and subjects. 
3. **Apply Label:**
   Enter the message ID and the label you want to apply to the email.

## Additional Notes 
- The script uses the `gmail.modify` scope to perform label-related operations.
- Labels not found during label application will prompt you to create a new label.

## Contributions
Contributions and improvements are welcome. Feel free to submit issues or pull requests.

## License
This project is licensed under the [MIT License](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt) 
