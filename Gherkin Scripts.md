# Test Scripts #

### (TC001): User logs in, updates profile and logs out successfully ###

* **Given** the user navigates to the login page
* **When** the user enters valid credentials
* **And** clicks the “login” button
* **Then** the user should be redirected to the dashboard
* **When** the user navigates to the “Edit Profile” page
* **And** updates their profile with valid information
* **And** clicks the “Save” button
* **Then** the user should see a confirmation message
* **And** the profile should reflect the updated information
* **When** the user clicks “Logout” button
* **Then** the user should be logged out
* **And** redirected to the login page

### (TC002): Login to protected resource with invalid token ###

* **Given** the user has an invalid authentication token
* **When** the user sends a request to a protected endpoint
* **Then** the system should respond with status 401
* **And** return an error message stating “invalid API Key”

### (TC003): User attempts to update profile with missing required fields ###

* **Given** the user is logged into the application
* **And** the user navigates to the "Edit Profile" page
* **When** the user leaves required fields blank And clicks the "Save" button
* **Then** the system should display validation error messages
* **And** the profile should not be updated 

###  (TC004) : Fetch user list using invalid pagination parameters ###

* **Given** the API endpoint “/users” supports pagination with “page” and “limit”  
           parameters
* **When** the user sends a GET request with “1” and “0”
* **Then** the system should respond with status code  “400”
* **And** the response body should include an error message “Limit must be greater 
               than 0”



