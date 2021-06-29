# Documentation
The Edge API allows business users to collect data from their beacon.

# Getting Started
**Step 1**:
If you haven't already, please sign up for an account through the Edge website: http://edge-app-client.epizy.com/sign-up.

![image](https://user-images.githubusercontent.com/86634813/123722156-9edf3e00-d83c-11eb-935d-7537fb1ce7d4.png)

**Step 2**:
Once your business account has been created, you're ready to start collecting data. Data can be collected through the following HTTP request:
`http://165.232.143.117:8000/api/get-users-nearby/`

**Parameters:**

`username`: The username for your business account.

`password`: The password to your business account.

**Returns:** A list of dictionaries containing data for each user. For more information about the type of data you can collect, please see the "User Data" section.

![image](https://user-images.githubusercontent.com/86634813/123723359-16ae6800-d83f-11eb-8ba9-502dc7a61ff3.png)
(Making a request for data in Python)

# User Data
Users may have any of the following fields. If a data-point is unavailable for a given user, its value will be undefined, but still exist in the user's dictionary (`None`, `null`, etc.).

`first_name`: A user's first name.
Example: "Braxton"

`last_name`: A user's last name.
Example: "Garcia",

`location`: A user's GPS location in the format `longitude, latitude`.
Example: "39.732598848245885, -104.98701590248902"
