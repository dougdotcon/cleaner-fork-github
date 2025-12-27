# GitHub Fork Cleaner

A comprehensive tool designed to efficiently manage and clean up your forked GitHub repositories using a modern graphical user interface.

## Features

- **Modern GUI Interface:** Intuitive graphical interface built with Python for ease of use.
- **Repository Visualization:** View all your forked repositories in a centralized dashboard.
- **Smart Deletion:** Automatically adds a star to a repository before deleting the fork, preserving history.
- **Secure Credential Management:** Safe handling of GitHub credentials using environment variables.
- **Progress Tracking:** Real-time visual feedback on the status of operations.

## Prerequisites

- Python 3.7 or higher
- A GitHub Personal Access Token with the following permissions:
  - `repo` (Full control of private repositories)
  - `delete_repo` (ToDelete repositories)

## Installation

### 1. Clone the Repository

bash
git clone https://github.com/your-username/github_fork_cleaner.git
cd github_fork_cleaner


### 2. Install Dependencies

It is highly recommended to use a virtual environment:

bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt


### 3. Configure Credentials

Rename the example environment file:

bash
mv .env.example .env


Edit `.env` and add your GitHub details:

ini
GITHUB_USERNAME=your_github_username
GITHUB_TOKEN=your_github_personal_access_token


## Usage

### Recommended: Graphical User Interface (GUI)

Run the main application to launch the GUI:

bash
python app_gui.py


**The GUI allows you to:**
- Configure credentials securely.
- Fetch and list all your forks.
- Select specific forks to remove.
- Monitor the progress of deletion tasks.

### Alternative: Command Line Interface (CLI)

If you prefer the terminal, run the CLI version:

bash
python app.py


## Security Best Practices

- **Never commit your `.env` file** or push it to version control.
- **Limit Token Permissions:** Ensure your GitHub token only has the necessary scopes (`repo`, `delete_repo`).
- **Keep Credentials Safe:** Do not share your token or username publicly.

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.
