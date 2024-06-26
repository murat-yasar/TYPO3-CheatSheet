# Create A Typo3 Project

## 0. Requirements

## 1. Install
[TYPO3 Install Guide](https://docs.typo3.org/m/typo3/tutorial-getting-started/12.4/en-us/Installation/Install.html#or-use-the-gui-installer-in-the-browser)

1. Install project with Composer
```bash
   composer create-project typo3/cms-base-distribution <project-name> "^12"
```

2. Get into the project directory
```bash
   cd <project-name>
```
   
4. Install DDEV
```bash
   ddev config --project-type=typo3 --docroot=public --php-version 8.3
```

3. Start DDEV
```bash
   ddev start
```

4. Initialize Configuration
```bash
   touch public/FIRST_INSTALL
```

5. Open the project in your web browser (open through Docker)
   > [Web Browser]: <localhost>/typo3/install.php

6. Set username, password, etc.
   > [Web Browser]: <localhost>/typo3/install.php

7. Access the Page
   > [Web Browser]: <localhost>/typo3
