# Kickoff
Author: Si Jobling ([@Si](http://twitter.com/Si))

Collaborators: Brian Suda ([@briansuda](http://twitter.com/briansuda)), Andy Higgs ([@aajhiggs](http://twitter.com/aajhiggs))

## Project goal
Provide usable, engaging data for sports events

## Target - Summer 2015
 
 * **Rugby World Cup 2015** in England & Wales - _September 2015_
 * **FA 2015-16** football season (FA Cup, Premiership, Championship, League 1 and 2) - **August 2015**

## Legacy Products

 * [World Cup Kickoff](http://worldcupkickoff.com)
 * [6 Nations Kickoff](http://6nationskickoff.com)
 * [Rugby World Cup Kickoff](http://rugbyworldcupkickoff.com)
 * [F1 Calendar](http://worldcupkickoff.com)
 * [UEFA Calendars](http://calendars.uefa.com)

## Features
### Consumption

 * **Discover** - popular and search
	* **Football** - Premier League, Championship, internationals
	* **Motors** - Formula 1, MotoGP (Bikes)
	* **Rugby** - 6 Nations, International, World Cup 2015!
	* **Tennis** - Wimbledon, opens
	* **Cycling** - Tour De France
 * **Calendar View** - view of all events, either as calendar grid or timeline (feed) list
 * **Competition Calendar Subscriptions** - ICS calendar file/subscription grouped by a competition
	* **Instructions per application** - Outlook (different versions), Mac, Google Calendar, iOS
 * **Reminders with custom durations** - hour/day/week before
	* Emails
	* Social updates
	* Tweets with hashtags eg. #sport #team
	* Facebook page updates with hashtags
	* Google+
	* Push Notifications API
 * **Open data** - Web API using common formats
 	* XML
	* JSON
	* RSS feeds of events
 * **Share calendars** – invite people to see the calendar
 	* Email
 	* Tweet
 	* Share on FB
 * **Mobile first** - desktop secondary (it's all about context and ease of access)
 * **Ofline capability** 

### Curation

 * **Calendars** – create and manage calendars
 	* **Residency** – location with map
 	* **Reminders** – duration, frequency
 	* **Meta** – customisable additional content
 	* **Access** - public, private or invited
 * **Events** – create, edit, remove
	* **Summary** – club names with results
 	* **Opponents** – teams with logos
 	* **Dates** – dates
 	* **Times** – optional times or "all day"
 	* **Venue** – location with map, default to first team residency
 	* **Details** – additional information, custom key/value meta
 * **Moments** – key events within events
 	* **Goals** – player, time
 	* **Fouls** – reference all players
 	* **Benchmarks** – half time, full time
 	* **Source** – URL, commentator
 * **Locations** – create, edit, flag
	* **Name**
	* **Location** – address, postcode, long/lat
	* **Contact details** – telephone, email
	* **Social** – connect with Google, Facebook, Twitter, Foursquare, 
 * **Teams** - create, edit, flag
	* **Profile** – name, badge
	* **Residency** – location with map
	* **Social** – connect with Twitter, Facebook, Instagram
 * **Players** - create, edit, flag
	* **Profile** – name, dob, number
	* **Social** – connect with Twitter, Facebook, Instagram
 * **Users** 
	* **Register or Sign in** – email and password or social
	* **Profile** – name, photo, location, username
	* **Social** – connect with Twitter, Facebook, Instagram etc
	* **Permissions** – player, team, events, calendars
	* **Friends** – discover or invite friends on social

## Thoughts

 * Isolate core elements as workflows/processes
 * Configure processes to personal requirements
	* IFTTT > push notifications, emails
 * Generate fan-based commentary for events from dedicated Twitter accounts ([@derbycounty](http://twitter.com/derbycounty)) or hashtags (_#dcfcfans_)
 * Include rich media from other social networks
	* Instagram
	* Snapchat
	* Periscope!

 * Source event activity (match goals) from white list of official Twitter accounts with custom regexp
	* [@dcfcofficial](http://twitter.com/dcfcofficial)
	* [@official_nffc](http://twitter.com/official_nffc)
 * Source FA fixtures from reliable content scrape (BBC)
 * Mini services spun up on Heroku (small free accounts) for sourcing and providing content 
	* FIFA to Data
	* FA to Data
	* Derby County to Data
	* F1 to Data
	* Data to ICS
	* Data to JSON
	* Data to RSS
	* Data to IFTTT

## Promotion

 * Tutorials for users 
 * Press releases for utilising content with hot gadgets
	* Little Printer
	* Apple Watch
	* Internet of Things (IoT)
 * Dedicated apps for specific competitions/sports
 * Hackathon events with developers
 * Engaging with local sport clubs and communities, offering managed services and training
 * Recruit someone with marketing expertise and background
 * Migrate UEFA to new platform and PR spin

## Press Releases

 * Producthunt
 * Techcrunch
 * Reddit
 * 
