# clickstream-route-finder
Analyze user routes within website sessions using Apache Spark, identifying the most frequent paths users take through the site.

# Description
__Clickstream__ is a sequence of user actions on a website, allowing understanding of user interactions with the site. The goal of this repository is to identify the most frequent custom routes users take through the site, using various interfaces like Spark SQL, Spark RDD, and Spark DF.

## Input Data
The clickstream data is stored in a CSV file with the following structure:

* `user_id`: Unique user identifier (int).
* `session_id`: Unique identifier for the user session (int).
* `event_type`: Event type (string) – "page", "event", or a custom string.
* `event_page`: The page on the site where the event occurred (string).
* `timestamp`: Unix-timestamp of the action (int).
