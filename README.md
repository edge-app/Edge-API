# Documentation
The Edge API allows business users to collect data from their beacon.

# Getting Started
Step 1:
If you haven't already, please sign up for an account through the Edge website: http://edge-app.epizy.com/#contact-us.

Step 2:
Once your business account is created, you're ready to start collecting data. Data can be collected through the following HTTP request:
`http://165.232.143.117:8000/api/get-users-nearby/`
  Returns: A list of dictionaries containing data for each user. For more information about the type of data you can collect, please see the "User Data" section.

# User Data
Users may have any of the following fields. If a data-point is unavailable for a given user, its value will be undefined, but still exist in the user's dictionary (`None`, `null`, etc.).

`first_name`: A user's first name.

Examples: "Braxton", "Eisa", "Sonnie"

`last_name`: A user's last name.

Examples: "Valencia", "Weber", "Garcia",

`location`: A user's GPS location in the format `longitude, latitude`.

Example: "39.732598848245885, -104.98701590248902"
