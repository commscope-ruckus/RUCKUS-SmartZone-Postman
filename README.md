# SmartZone-Postman
Postman collections containing many API call sequences to perform configuration tasks on SmartZone Controllers

Instructions

Edit the attribute values for the API call "1. Get service ticket" under the folder "System" to match with your vSZ instance:

- change the IP address in the "Pre-request Script"
- change the credentials in the "Body"

Check if if system clock in your vSZ instance matches the clock in your computer. Make the necessary adjustments (sync the NTP server or change the time zone), otherwise the API calls that are time-dependent (ex: "2. Get wireless application traffic" under "Clients and Traffic") will not return the correct values.

Send the API call "1. Get service ticket" to obtain the authentication token.
Send each of the subsequent API calls in the order which they appear.

After you execute all calls, clean you vSZ instance by executing all API calls under the "Delete objects" folder, in the order which they appear.
You can see the variable values in the "Variables" tab in this page.
For more information about this collection please contact marcelo.molinari@commscope.com
