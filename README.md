# WDLookup Queries

This is a library of WQL queries. The queries can be used generally with any WQL tool or with the WDLookup Excel Add-in (Windows only).

Anyone is welcome to contribute to this library. Submit a pull request for review.  If you do not know how to submit a pull request, paste the query into a discussion post and mention that you would like it added to the library. Please follow the query examples to include information about the query (name, description, etc.).  In the future, there are plans to parse the files and enable an electronic dictionary.

Use the **Convert Report to WQL** report to get a headstart with query generation.  This report will generate WQL from existing Workday reports.

![image](https://user-images.githubusercontent.com/413552/144367130-94258363-2f81-4a62-bc8d-dccfe544e79e.png)


If you will be using the WDLookup Excel Add-in, the configuration instructions are shown below.


# WDLookup Excel Add-in

WDLookup is a Microsoft Excel Add-in (Windows only) that enables querying data from Workday using WQL.

If you would like to use WDLookup to execute the queries from this library, download and install WDLookup from the following link. 

**https://whitleymedia.onfastspring.com/**

**IMPORTANT:** The add-in is fully-functional except that it is limited to returning *10 rows of data per query*. This limitation can affect your ability to translate data using the **Lookup** feature.  Remember that only the first 10 rows of the lookup query are returned so data outside of the first 10 rows cannot be translated. 

Purchase a registration code to unlock the ability to return all rows of data.

## Workday API Client Setup for WDLookup

WDLookup requires an API client connection for Workday.  This is a one-time setup requirement and requires less time than you think. ;)

The following pieces of information need to be collected during these steps:

:heavy_check_mark: Workday REST API Endpoint

:heavy_check_mark: Token Endpoint

:heavy_check_mark: Client ID

:heavy_check_mark: Client Secret

:heavy_check_mark: Refresh Token

### Let's Get Started

#### In your Workday tenant...

1. Turn on oAuth 2.0

    **Search for Task:** Edit Tenant Setup - Security

![image](https://user-images.githubusercontent.com/413552/142732206-bfdcf00e-b7f9-42f7-a841-5c2836be95cd.png)

2. Register an API Client for Integrations

    **Search for Task:** Register API Client for Integrations

      a. Check **Non-Expiring Refresh Tokens**.

      b. Select **System** for the Scope.

      c. Click OK.

      d. On the next screen, scroll to the bottom of the page.

      e. Copy your *Client ID* and *Client Secret* so that they can be used later.

![image](https://user-images.githubusercontent.com/413552/142732320-f7f3a7d5-a851-4d50-889d-c54e84706012.png)

3. View API Clients

    **Search for Task:**  View API Clients

    Save the following urls for later:
    
        - Workday REST API Endpoint
        - Token Endpoint

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
1. In Excel, from the **Add-ins** menu, start **WDLookup**.
2. Click the **WDLookup Settings** button. 

   <img src="https://user-images.githubusercontent.com/413552/142780606-39f4fbb3-4709-4cf2-893a-d9d4762ddcfe.png" width="32" />
3. If the Name is not already set to "{New}", click the **Add API Client** button.
4. Name your API Client. You can use any name that makes sense to you.
5. Enter the API Client information from Workday.
6. Leave **Access Token** blank.
7. Click **Save** to save the API Client.
8. Click **Test** to verify a successful connection to Workday.

![image](https://user-images.githubusercontent.com/413552/142780581-543f2cf9-9a71-49b3-b38a-1aeff4dca98c.png)

### Running a Query

1. Enter a WQL query into the query textbox.
2. Click the **Run** button.
3. The query results will be pasted into the active Excel worksheet.
4. Please note that existing data in the spreadsheet will be cleared to make way for the query data.

 ![image](https://user-images.githubusercontent.com/413552/143399956-041fff33-29ce-44e9-ab8e-7e9f39ae4832.png)


### Performing a Lookup and Reverse Lookup

WDLookup has a handy right-click menu that will execute the currently displayed query.

Remember, if you are using the unregistered version of WDLookup, only 10 rows of data will be returned. This applies to the lookup as well.  For example, you may be able to perform a lookup on a country that starts with "A", but a country that starts with "U" may not be returned and translated.  

The query results will be used to lookup the data in the highlighted cells and translate the data if it matches the first column of the query.  The translation will update each selected cell with data from the second column in the query.  If a translation cannot be made, the cell will be highlighted in yellow.

The reverse lookup feature reverses the process without any change to the query.  The reverse lookup performs a lookup in reverse (the second field is the selector and the first field is the translation); it does not simply undo the results of the previous operation.


[![Watch the video](https://img.youtube.com/vi/bCCusSF4GGA/maxresdefault.jpg)](https://www.youtube.com/watch?v=bCCusSF4GGA)


### Registering WDLookup

Unlock WDLookup's ability to retrieve more than 10 rows of data by purchasing a registration code at the following link:

**https://whitleymedia.onfastspring.com/**

Follow the steps below to register WDLookup.

1. Click on the button to show the registration page.

![image](https://user-images.githubusercontent.com/413552/143470768-ad0445d9-12ad-4c49-95fc-4e772f144cbf.png)

2. Enter the email address that was used to purchase the registration code.
3. Paste the registration code into the registration code textbox.
4. Click the **Save** button.  A dialog box will appear to confirm that WDLookup has been successfully registered.

![image](https://user-images.githubusercontent.com/413552/143471980-6a0d88e4-116a-4769-b4f4-3567a30d4b6c.png)


