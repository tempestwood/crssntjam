# Crssnt Jam

Free RSS aggregator - filter out the cruft.

Crssnt Jam is a Google Sheet that aggregates RSS feeds and filters feed items based on simple search terms - you can include and exclude terms at the same time.

Use [Crssnt](https://crssnt.com) to convert your Crssnt Jam Sheet into an RSS feed and subscribe to it with your favorite RSS reader or service.

## How Crssnt Jam works

Crssnt uses a script to build up a native Sheets query function when you add or remove feeds or alter the search terms in your configuration. Once you have it configured how you like, it is refreshed automatically when requested by Crssnt.

## Install

1. [Copy Crssnt Jam](https://docs.google.com/spreadsheets/d/1IHfA5q1DZfq2PZ5vz39eim3VxhiOKbBHNU_Wqz7nJfM/copy) to your own account.
2. Click on `Tools > Script Editor`.
3. Run the script once to set the permissions for the script to access your Sheet on Google Drive. You may see an [unverified app](https://support.google.com/cloud/answer/7454865) warning. Follow the prompts and agree to allow the script to run - you are giving permission to your own Google account to access your own Sheet.
4. Click `File > Share` to set view permissions for anyone with the link to the Sheet - Crssnt needs view permissions to generate the RSS feed. 

## Configure your feeds

Select the `config` sheet follow the example provided by the feeds in the sheet.

For each feed you want to subscribe to enter the following under the column headings:

- 	**URL** the feed url you are subscribing to
- 	**Include Keywords** pipe delimited lowercase keywords to include e.g. `iphone 12 pro|airtags`
- 	**Exclude Keywords** pipe delimited lowercase keywords to exclude e.g. `wall st|deals:|opinion:`
- 	**Has Author** TRUE or FALSE

**Note:** until the value for Has Author is automated you will manually need to set the value. After entering the url, check the `Raw` sheet to see if the authors name is where the URL should be and set the Has Author value to TRUE, otherwise set it to FALSE.

## Subscribing to your feed

Use the Feed URL on the `config` sheet to subscribe to your new RSS feed. Update the feed name to something more meaningful in your feed reader.
