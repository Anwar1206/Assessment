## QA Assignment ##

This README provides steps to:

- Import and run Postman collections for API testing
- Perform mobile responsive testing on Chrome
- Prerequisites (Chrome browser, Android Studio, Postman version)
- Set up required tools and environments

Before you begin, make sure you have:

-  [Postman](https://www.postman.com/downloads/) installed
-  [Google Chrome](https://www.google.com/chrome/) updated to latest version
-  Access to API endpoints and sample payloads (if private)
-  Postman collection `.json` file exported from source project

How to Import and Run Postman Collection:

* Launch Postman
* Click **Import** in the top-left corner
* Drag and drop or browse for the `.json` collection file (Assessment.postman_collection.json)
* Drag and drop or browse for the `.json` environment file (Testing Env.postman_environment.json)
* Collection appears in the **Sidebar**
* Expand the collection and select a request
* Click **Send** to run it
* Review **Response**, **Headers**, and **Status Code**

How to perform Mobile Responsive Testing on Chrome:

1. Open the website(www.zara.com) in Google Chrome
2. Right-click on the page and select **Inspect**
3. Click the **Toggle device toolbar** (icon in top-left of DevTools)
4. Choose a device from the drop-down menu (iPhone X, Pixel 2)
5. Refresh the page to load CSS styles properly
6. Interact with the site to validate:
   -  Layout shifts
   -  Touch targets
   -  Font size and visibility
   -  Button alignment
7. Change device orientation by clicking the rotate icon

How to find a file in repo:

* Go to the repo
* Press 't' on your keyboard - this opens the **File Finder**
* Start typing the file name - Gherkin Scripts or Mobile_defects
