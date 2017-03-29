Drip API Wrapper - PHP
===============

An object-oriented PHP wrapper for Drip's REST API v2.0

2017-03-29 Changes
--

Move towards getters and setters for setting and accessing object data.
You can now set the working account ID using `setAccountId()` instead of
having to set it as a param to each function.
 
Can also set API Token using `setApiToken()` and there
 is no dependency for having API token at the time of
 API construction, meaning you can also switch API token
 if this is ever required. (An exception is still thrown
 for empty API token but this will be triggers at the 
 moment of API query sending and not object construction.)

Added 3x new API wrapper methods:
* `fetch_subscribers()` fetches all subscribers for a given page
* `fetch_all_subscribers()` fetches all subscribers for an account
* `subscriber_delete()` deletes an individual subscriber 