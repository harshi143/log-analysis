# log-analysis
1. Count Requests per IP Address
Purpose: Analyze the frequency of requests made by each IP address in the log file.
Methodology:
Extracts IP addresses using regex patterns.
Counts occurrences of each IP address using the collections.Counter module.
Sorts and displays the results in descending order of request count.
Output Format:
Displays a table listing IP addresses alongside their respective request counts in the terminal.
2. Identify the Most Frequently Accessed Endpoint
Purpose: Determine the endpoint (URL or resource path) that has been accessed the highest number of times.
Methodology:
Extracts endpoints from HTTP requests using regex patterns.
Uses Counter to track the frequency of each endpoint.
Identifies and displays the most accessed endpoint along with its count.
Output Format:
Displays the most frequently accessed endpoint in the terminal.
Detect Suspicious Activity
Purpose: Identify potential brute force login attempts by detecting repeated failed login attempts from specific IP addresses.
Methodology:
Searches for failed login attempts using HTTP status code 401 or a failure message such as "Invalid credentials".
Counts failed login attempts per IP address using Counter.
Flags IPs exceeding a configurable threshold (default: 10 failed attempts).
Output Format:
Lists flagged IP addresses with their failed login counts in the terminal.

