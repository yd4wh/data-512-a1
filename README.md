# data-512-a1

### Project Goal:
English Wikipedia has API that can track pageviews of desktop site and mobile site, this project will pull the pageview data from English Wikipedia's API and graph out the trend from December 2007 thru September 2018.

### Source Data:

ALl source data is from REST API, all content accessed via this API is licensed under the CC-BY-SA 3.0 and GFDL licenses.

See API documentation here: https://en.wikipedia.org/api/rest_v1/

Wikimedia Foundation REST API terms of use: https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions

### Final Data:

`year`: the year in which these pageviews are generated

`month`: the month in which these pageviews are generated

`pagecount_all_views`: all the legacy pagecount from both desktop site and mobile site

`pagecount_desktop_views`: legacy pagecount from desktop site only

`pagecount_mobile_views`: legacy pagecount from mobile site only

`pageview_all_views`: all update method pageview from both desktop site and mobile site

`pageview_desktop_views`: update method pageview from desktop site

`pageview_mobile_views`: update method pageview from mobile site

### Note about the data:
Pagecount information are from legacy data collection, which spans from December 2007 thru July 2016 for desktop site and from October 2014 thru July 2016 for mobile site.

Pageview information are from updated data collection, which spans from July 2015 thru recent month(September 2018) for both desktop and mobile site. This updated data collection distinguish humans from robotic traffic and mark them in separate column as agent('users' or 'crawlers'). For our analysis, we limited agent to human users only. The original Pagecounts API does not distinguish the two.
