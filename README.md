# Desktop Cleaner
Desktop Cleaner is a Python script designed to automatically organize files on your desktop into categorized folders based on their file extensions. It utilizes the Watchdog library to monitor changes on the desktop directory and moves files to appropriate folders according to predefined extension paths.

# Usage
1. Run the main.py script. This will start monitoring your desktop directory for file changes.
2. Files on your desktop will be automatically moved to categorized folders based on their file extensions.
# File Structure
- main.py: The main script that initializes the file monitoring process and sets up the event handler.
- extensions.py: Defines a dictionary mapping file extensions to their respective destination folders.
- EventHandler.py: Contains the EventHandler class responsible for handling file system events and organizing files based on their extensions.

# Customization
- You can customize the destination folders for specific file extensions by modifying the extensions.py file.
- Add or remove file extensions and their corresponding destination paths as needed.
- The add_date_to_path function in EventHandler.py adds the current year and month to the destination path for better organization of files.
- The rename_file function in EventHandler.py ensures that files with conflicting names are renamed to prevent overwriting existing files.
