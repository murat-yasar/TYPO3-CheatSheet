# Start A Typo3 Project

## 0. Requirements

## 1. Install
[TYPO3 Install Guide](https://docs.typo3.org/m/typo3/tutorial-getting-started/12.4/en-us/Installation/Install.html#or-use-the-gui-installer-in-the-browser)

1. Create the project directory
```bash
   mkdir my-t3-project
   cd my-t3-project
```

2. Install project with DDEV
```bash
   ddev config --php-version 8.3
```

3. Configure Project
```bash
   # Give the following answers when prompted:

   # Project name (t3example):
   # Docroot Location (current directory):
   public
   # Project Type [php, typo3, ...] (php): 
   typo3
```

4. Start DDEV
```bash
   ddev start
```

5. Install server with GUI
```bash
   touch /public/FIRST_INSTALL
```

6. Access TYPO3 via a web browser (Set username, password, etc.)
Web Browser:  http://127.0.0.1:50503/typo3/install.php
