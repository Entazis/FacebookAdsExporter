# Facebook Ads Exporter with Slack notifications 

* Export Facebook Ads Data in Spreadsheet with the help of DIY sheet add-on.
* Check Here for Setup: https://www.digishuffle.com/blogs/cost-data-import-facebook-to-google-analytics/
* Check Here for UI Help: https://www.digishuffle.com/free-facebook-ads-reporting-tool/

This project was made for a company using `RitwikGA/FacebookReportingTool` to export daily, weekly, monthly facebook ads.
The project runs on script.google.com and exports and saves these fields for each campaign for each period in a spreadsheet:
* Start Date
* End Date
* Locale
* Campaign name
* Cost
* Impressions
* Clicks
* Avg. pos.
* Number of new trial users from this campaign
* Number of new paying users from this campaign

It also updates the data from earlier exports.

At the end of each export, the exported data is also sent to a Slack channel.

There are 3 functions that can be set to run daily/ weekly/ monthly, each of them exports facebook ads for that period starting from the last exported date:
* `facebookDataDaily()`
* `facebookDataWeekly()` 
* `facebookDataMonthly()`