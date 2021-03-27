# Crssnt Jam

Free RSS aggregator - filter out the cruft.

Crssnt Jam is a Google Sheet that aggregates RSS feeds and filters feed items based on simple search terms - you can include and exclude terms at the same time.

Use [Crssnt](https://crssnt.com) to convert your Crssnt Jam Sheet into an RSS feed and subscribe to it with your favorite RSS reader or service.

## How Crssnt Jam works

Crssnt uses a script to build up a native Sheets query function when you add or remove feeds or alter the search terms in your configuration. Once you have it configured how you like, it is refreshed automatically when requested by Crssnt.

## How to use

1. [Copy Crssnt Jam](https://docs.google.com/spreadsheets/d/1IHfA5q1DZfq2PZ5vz39eim3VxhiOKbBHNU_Wqz7nJfM/copy) to your own account.

2. Click on `Tools > Script Editor`.

3. Run the script once to set the permissions for the script to access your Sheet on Google Drive. You may see an [unverified app](https://support.google.com/cloud/answer/7454865) warning. Follow the prompts and agree to allow the script to run - you are giving permission to your own Google account to access your own Sheet.

4. Edit the configuration in the `config` sheet. Enter the URL, a pipe separated list of keywords to include, a pipe separated list of keywords to exclude, and TRUE or FALSE depending on if the feed you are subscribing to has an Author column. Until this is automated you will manually need to set the value - after entering the url, check the Raw worksheet to see if the authors name is where the URL should be and set the Has Author value to TRUE, otherwise set it to FALSE.

5. Click `File > Share` to set view permissions for anyone with the link to the Sheet - Crssnt needs view permissions to generate the RSS feed.

6. Follow the instructions on [Crssnt](https://crssnt.com) to create your RSS feed url.


		

