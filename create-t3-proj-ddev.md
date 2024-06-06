# Start A Typo3 Project

## 0. Requirements

## 1. Install
[TYPO3 Install Guide](https://docs.typo3.org/m/typo3/tutorial-getting-started/12.4/en-us/Installation/Install.html#or-use-the-gui-installer-in-the-browser)

1. Create the project directory
```bash
   mkdir <project-name>
   cd <project-name>
```

2. Install project with DDEV
```bash
   ddev config --php-version 8.3
```

3. Configure Project
```bash
   ddev config
   # Give the following answers when prompted:

   # Project name (t3example):
   # Docroot Location (current directory):
   public
   # Create docroot .../public?:
   Y
   # Project Type [php, typo3, ...] (php): 
   typo3
```

4. Start DDEV
```bash
   ddev start
```

5. Install server with GUI
```bash
   touch public/FIRST_INSTALL
```

6. Access TYPO3 via a web browser
   Web Browser:  <localhost>/typo3/install.php

7. Set admin configuration (username, password, etc
   Web Browser:  <localhost>/typo3/install.php
