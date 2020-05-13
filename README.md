<h2>Data Modeling with Postgres for Sparkify<h2>

![Image of post](postgres.png)

<h3>Introduction:<h3>

<p>An music streaming startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.<p>

<p>Create a Postgres database with tables designed to optimize queries on song play analysis. The task is to create a star schema for Postgres and develop an ETL pipleine which will transfer the data from local files to the database.<p>

<h3>Data:<h3>
   
<p>The songs metadata derives from the Million Song Dataset which consists of the songs' features.<p> 

<p>The users' activity metadata (log data) is known to be a simulated data using eventsim. This data is composed of daily user's activities on the music streaming app.<p> 

<h3>Requirements when running locally:<h3>
 
<ol>
<li>Python3</li>
<li>Dockr</li>
<li>Docker-Compose</li>
    </ol>


<h3>Database Star Schema:<h3>

![Image of Schema](schema.png)

<h3>Source Code:<h3>

<ol>
<li>create_table.py establishes the connection, creates and drops tables while creating the database.</li>
<li>etl.py builds the ETL pipeline that will convert raw data into a format compataible with the database tables.</li> 
<li>sql_queries.py lists all of the queries to create, insert, and drop the tables for the database.</li>
    </ol>




