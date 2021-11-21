# WDLookup Queries

This is a library of WQL queries. They can be used generally with any WQL tool or with the WDLookup Excel Add-in.

If you will be using the WDLookup Excel Add-in, the configuration instructions are show below.

## Workday API Client Setup
WDLookup requires an API client connection for Workday.  This is a one-time setup requirement and requires less time than you think. ;)

In your Workday tenant...

1. Turn on oAuth 2.0

**Task:** Edit Tenant Setup - Security

![image](https://user-images.githubusercontent.com/413552/142732206-bfdcf00e-b7f9-42f7-a841-5c2836be95cd.png)

2. Register an API Client

**Task:** Register API Client for Integrations

![image](https://user-images.githubusercontent.com/413552/142732320-f7f3a7d5-a851-4d50-889d-c54e84706012.png)

3. Click OK.  On the next screen, scroll to the bottom of the page.  Copy your *Client ID* and *Client Secret* so that they can be used later.
4. View API Clients

**Task:**  View API Clients

Save the following urls for later:
* Workday REST API Endpoint
* Token Endpoint

5. Click the **API Clients for Integrations** tab
6. Click on the link for your newly created API Client.
7. Use the related action to click **Manage Refresh Tokens for Integrations**.

![image](https://user-images.githubusercontent.com/413552/142732556-152d8dad-e806-4bfb-8598-9cbe2ea87b31.png)

8. Associate a Workday user with the API Client.

![image](https://user-images.githubusercontent.com/413552/142732607-d5489b7d-9984-4aa9-a826-8316a95c9190.png)

9. At the bottom of the page, select **Generate New Refresh Token**

![image](https://user-images.githubusercontent.com/413552/142732666-65b716e6-b42e-4d3a-84dc-87f8c4073200.png)

10. Copy and save the refresh token for later.


## WDLookup
