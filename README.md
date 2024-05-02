# HubSpot Email Marketing SpotApp

SpotApps are ThoughtSpot’s out-of-the-box solution templates built for specific use cases and data sources. They utilize ThoughtSpot Modeling Language (TML) Blocks, which are pre-built pieces of code that are easy to download and implement directly from the product.

The HubSpot Email Marketing SpotApp mimics the HubSpot data model. When deployed, it creates several Worksheets, Answers, and Liveboards based on your HubSpot data in your cloud data warehouse.

Use the HubSpot Email Marketing SpotApp to identify the success of your email campaigns. Determine which emails are working, and use that information to make data-driven decisions about where to focus your marketing budget.


## Overview

Use the HubSpot Email Marketing SpotApp to identify the success of your email campaigns. Determine which emails are effective and use that insight to make data-driven decisions about where to focus your marketing budget.

## Prerequisites

Before you can deploy the HubSpot Email Marketing SpotApp, you must complete the following prerequisites:

- **Review Required Data**: Examine the required tables and columns for the SpotApp.
- **Ensure Column Compatibility**: Make sure that your columns match the required column type listed in the schema for your SpotApp.
- **Sync Data**: Synchronize all tables and columns from HubSpot to your cloud data warehouse. While you can choose to sync only the required tables and columns, ThoughtSpot recommends syncing all tables and columns from HubSpot to ensure comprehensive data availability. This includes HubSpot’s out-of-the-box columns or any custom columns you are using.
- **Collaborate on Data Movement**: If you are using an ETL/ELT tool or working with another team within your organization, sync all columns from the tables listed in the SpotApp.
- **Obtain Credentials**: Obtain credentials and SYSADMIN privileges to connect to your cloud data warehouse. The warehouse must contain the data ThoughtSpot will use to create Answers, Liveboards, and Worksheets.
- **Unique Connection Name**: Each new SpotApp connection name must be unique.
- **Super Admin Access to HubSpot**: Maintain Super Admin access to manage HubSpot resources.
- **Access to HubSpot Tables**: Ensure access to the following HubSpot tables in your cloud data warehouse:
  - `HUBSPOT_MARKETING_EMAIL`
  - `HUBSPOT_MARKETING_EMAIL_EVENTS`

### Run SQL Commands

Execute the necessary SQL commands in your cloud data warehouse to standardize data types and column names. Modify the code as necessary for your specific cloud data warehouse.

SQL Commands can be found here: https://github.com/thoughtspot/HubSpot-Email-Marketing-SpotApp/blob/main/HubSpot%20SQL%20Commands

## Deploy the SpotApp

## Deploy the SpotApp

After you have downloaded the Zip file and verified its contents, follow these steps:

1. Log into your ThoughtSpot instance and create an Embrace connection to all of the relevant views.
2. Import the TML for the Worksheets and verify that it has all been imported without any errors.
3. Import the TML for the Liveboards and verify that it has all been imported without any errors.
4. You are ready to start searching your data!

For detailed instructions on how to import TML files, refer to the [ThoughtSpot documentation](https://docs.thoughtspot.com/software/latest/tml-import-export-multiple).


For detailed instructions on how to import TML files, refer to the [ThoughtSpot documentation](https://docs.thoughtspot.com/software/latest/tml-import-export-multiple).
