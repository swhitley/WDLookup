# WDLookup Queries

This is a library of WQL queries. They can be used generally with any WQL tool or with the WDLookup Excel Add-in (Windows only).

Anyone is welcome to contribute to this library. Submit a pull request for review.  Please follow the example to include information about the query.  In the future, there are plans to parse the files and enable an electronic dictionary.

If you will be using the WDLookup Excel Add-in, the configuration instructions are show below.

## Workday API Client Setup
WDLookup requires an API client connection for Workday.  This is a one-time setup requirement and requires less time than you think. ;)

The following pieces of information need to be collected during these steps:

:heavy_check_mark: Workday REST API Endpoint

:heavy_check_mark: Token Endpoint

:heavy_check_mark: Client ID

:heavy_check_mark: Client Secret

:heavy_check_mark: Refresh Token

### Let's Get Started

In your Workday tenant...

1. Turn on oAuth 2.0

    **Task:** Edit Tenant Setup - Security

![image](https://user-images.githubusercontent.com/413552/142732206-bfdcf00e-b7f9-42f7-a841-5c2836be95cd.png)

2. Register an API Client for Integrations

    **Task:** Register API Client for Integrations

    a. Check **Non-Expiring Refresh Tokens**.

    b. Select **System** for the Scope.

    c. Click OK.

    d. On the next screen, scroll to the bottom of the page.

    e. Copy your *Client ID* and *Client Secret* so that they can be used later.

![image](https://user-images.githubusercontent.com/413552/142732320-f7f3a7d5-a851-4d50-889d-c54e84706012.png)

3. View API Clients

    **Task:**  View API Clients

    Save the following urls for later:
    
        * Workday REST API Endpoint
        * Token Endpoint

4. Click the **API Clients for Integrations** tab.
5. Click on the link for your newly created API Client.
6. Use the related action to click **API Client**, **Manage Refresh Tokens for Integrations**.

![image](https://user-images.githubusercontent.com/413552/142732556-152d8dad-e806-4bfb-8598-9cbe2ea87b31.png)

8. Associate a Workday user with the API Client.

![image](https://user-images.githubusercontent.com/413552/142732607-d5489b7d-9984-4aa9-a826-8316a95c9190.png)

9. At the bottom of the page, select **Generate New Refresh Token**.

![image](https://user-images.githubusercontent.com/413552/142732666-65b716e6-b42e-4d3a-84dc-87f8c4073200.png)

10. Copy and save the refresh token for later.

**Workday Configuration Complete**



## WDLookup Configuration

### Adding a new API Client
1. In Excel, from the **Add-ins** menu item, start **WDLookup**.
2. Click the **WDLookup Settings** button. 

   <img src="https://user-images.githubusercontent.com/413552/142780606-39f4fbb3-4709-4cf2-893a-d9d4762ddcfe.png" width="32" />
3. If the Name is not already set to "{New}", click the **Add API Client** button.
4. Enter the API Client information from Workday.
5. Leave **Access Token** blank.
6. Click **Save** to save the API Client.
7. Click **Test** to verify a successful connection to Workday.

![image](https://user-images.githubusercontent.com/413552/142780581-543f2cf9-9a71-49b3-b38a-1aeff4dca98c.png)

### Running a Query

TODO

### Performing a Lookup and Reverse Lookup

TODO





