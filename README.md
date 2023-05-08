Download Link: https://assignmentchef.com/product/solved-sdev-lab-10-heroku-website
<br>


 <main class="container" role="main"></main>

<p class="h5"><a href="./complete_student_site.zip">Download </a>the template and make sure you extract the files before using them.



5/5 - (1 vote)

<p class="lead">This lab will go over the steps needed to host our Node.js website and PostgreSQL database on Heroku. This lab is a “walk through” lab where the main focus is to ensure you can host your group project online. To receive credit for this lab, you MUST complete steps 1 and 3 in recitation and get marked off by your TA. You must upload “lab_10_link.txt” to Canvas by the deadline.

<table class="table">

 <tbody>

  <tr>

   <th class="h5">Est. Time &#x23f1;</th>

  </tr>

  <tr>

   <td class="h5"><span id="eta">0</span> minutes</td>

  </tr>

 </tbody>

</table>

<b><u>NOTE:</u></b> This lab is due next week Friday, 22nd Nov by 11:59pm.

<b><u>IMPORTANT:</u></b> Make sure you are logged into UCB Wireless, not UCB Guest. Otherwise the heroku pg:psql commands will fail !!

<p class="alignleft h5">Lab Overview

<button class="btn btn-primary btn-sm alignbtn" type="button">Mark Complete</button> <button class="btn btn-primary btn-sm alignbtn" type="button" data-toggle="collapse" data-target="#multiCollapseExample1" aria-expanded="false" aria-controls="multiCollapseExample1">Expand</button>

The abbreviated steps for todays lab are as follows:

<ol>

 <li>Regsiter for Heroku</li>

 <li>Create a new Heroku App</li>

 <li>Install Heroku CLI</li>

 <li>Upload the completed Node.js code to Heroku</li>

 <li>Setup PostgreSQL database on Heroku</li>

 <li>Submit a link to your Heroku App to Canvas</li>

</ol>




<p class="alignleft h5">1. Setup Heroku App

<p class="alignright h5">

<dl>

 <dt>

  <ul>

   <li>Register Heroku Account</li>

  </ul>

 </dt>

 <dd></dd>

</dl>

<hr>

<dl>

 <dt>

  <ul>

   <li>Create a New App</li>

  </ul>

 </dt>

 <dd>

  <hr>

  <hr>

 </dd>

 <dt>

  <ul>

   <li>Upload Node.js Website Code to Heroku</li>

  </ul>

 </dt>

 <dd>

  <hr>

 </dd>

</dl>

<img decoding="async" alt="Screenshot of Heroku Registration Page" data-src="img/heroku_register.png" class="img-fluid lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

<noscript>

 <img decoding="async" class="img-fluid" src="img/heroku_register.png" alt="Screenshot of Heroku Registration Page">

</noscript>

Go to Heroku’s Registration page <a href="https://signup.heroku.com/login" target="_blank" rel="noopener">here</a> and create an account.

<img decoding="async" alt="Screenshot of Heroku Dashboard Page" data-src="img/dashboard_heroku.png" class="img-fluid lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

<noscript>

 <img decoding="async" class="img-fluid" src="img/dashboard_heroku.png" alt="Screenshot of Heroku Dashboard Page">

</noscript>

Click on “Create New App”

<img decoding="async" alt="Screenshot of App Creation Page" data-src="img/heroku_create_app.png" class="img-fluid lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

<noscript>

 <img decoding="async" class="img-fluid" src="img/heroku_create_app.png" alt="Screenshot of App Creation Page">

</noscript>

Name your app, there is no required name here because every student submission will need to be a unique name.

<img decoding="async" alt="Screenshot of Heroku App Dashboard Page" data-src="img/heroku_app_dash.png" class="img-fluid lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

<noscript>

 <img decoding="async" class="img-fluid" src="img/heroku_app_dash.png" alt="Screenshot of Heroku App Dashboard Page">

</noscript>

Once you have named your app, you’ll be shown your Heroku App’s Dashboard.

To upload your code to Heroku, you’ll need to install the Heroku CLI.For Linux:

<pre class="command-line" data-user="csci3308" data-host="csci3308-VirtualBox"><code class="language-bash">sudo snap install --classic heroku</code></pre>

For Windows/Mac users, go <a href="https://devcenter.heroku.com/articles/heroku-cli" target="_blank" rel="noopener">here</a> to download the installer.

<img decoding="async" alt="Screenshot of instructions for uploading code to heroku" data-src="img/upload_code_heroku.png" class="img-fluid lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

<noscript>

 <img decoding="async" class="img-fluid" src="img/upload_code_heroku.png" alt="Screenshot of instructions for uploading code to heroku">

</noscript>

Follow the directions for your App Dashboard for connecting your website’s code to heroku.

<b><u>IMPORTANT:</u></b> Make sure that you follow the instructions from WITHIN the “complete_student_site” directory. If you haven’t already, download the complete_student_site.zip file and unzip it to your local machine.

<b><u>ALTERNATIVE:</u></b> If the website you created in <b>Lab 7</b> is working perfectly and there are no errors, you can upload it to Heroku instead of the complete_student_site we provided.

<pre class="command-line" data-user="csci3308" data-host="csci3308-VirtualBox"><code class="language-bash">heroku login</code></pre>

<pre class="command-line" data-user="csci3308" data-host="csci3308-VirtualBox"><code class="language-bash">git initheroku git:remote -a pick-unique-name-here</code></pre>

<pre class="command-line" data-user="csci3308" data-host="csci3308-VirtualBox"><code class="language-bash">git add .git commit -am "Initial Setup"git push heroku master</code></pre>

<p class="alignleft h5">2. Setup Heroku PostgreSQL Database

<button class="btn btn-primary btn-sm alignbtn" type="button">Mark Complete</button> <button class="btn btn-primary btn-sm alignbtn" type="button" data-toggle="collapse" data-target="#multiCollapseExample3" aria-expanded="false" aria-controls="multiCollapseExample3">Expand</button>

<p class="alignright h5">(<span id="time1" class="time">30</span> Minutes)

<dl>

 <dt>

  <ul>

   <li>Add a Heroku Resource</li>

  </ul>

 </dt>

 <dd></dd>

 <dt>

  <ul>

   <li>Connect to Heroku PostgreSQL Database</li>

  </ul>

 </dt>

 <dd>

  Make sure to replace “pick-unique-name-here” with the name of your actual heroku app.




  <pre class="command-line" data-user="csci3308" data-host="csci3308-VirtualBox"><code class="language-bash">heroku pg:psql -a pick-unique-name-here </code></pre>

 </dd>

 <dt>

  <ul>

   <li>Create the Database Tables</li>

  </ul>

 </dt>

 <dd>

  Copy the following code into psql terminal to create the football_player, footbal_games, and favorite_colors tables and populate them with data.




  <pre class="command-line" data-prompt="pick-unique-name-here::DATABASE="><code class="language-bash">DROP TABLE football_games;CREATE TABLE IF NOT EXISTS football_games (  visitor_name VARCHAR(30),       /* Name of the visiting team                     */  home_score SMALLINT NOT NULL,   /* Final score of the game for the Buffs         */  visitor_score SMALLINT NOT NULL,/* Final score of the game for the visiting team */  game_date DATE NOT NULL,        /* Date of the game                              */  players INT[] NOT NULL,         /* This array consists of the football player ids (basically a foreign key to the football_player.id) */  PRIMARY KEY(visitor_name, game_date) /* A game's unique primary key consists of the visitor_name &amp; the game date (this assumes you can't have multiple games against the same team in a single day) */);DROP TABLE football_players;CREATE TABLE IF NOT EXISTS football_players(  id SERIAL PRIMARY KEY,       /* Unique identifier for each player (it's possible multiple players have the same name/similiar information) */  name VARCHAR(50) NOT NULL,   /* The player's first &amp; last name */  year VARCHAR(3),             /* FSH - Freshman, SPH - Sophomore, JNR - Junior, SNR - Senior */  major VARCHAR(4),            /* The unique 4 character code used by CU Boulder to identify student majors (ex. CSCI, ATLS) */  passing_yards SMALLINT,      /* The number of passing yards in the players entire football career  */  rushing_yards SMALLINT,      /* The number of rushing yards in the players entire football career  */  receiving_yards SMALLINT,    /* The number of receiving yards in the players entire football career*/  img_src VARCHAR(200)         /* This is a file path (absolute or relative), that locates the player's profile image */);INSERT INTO football_games(visitor_name, home_score, visitor_score, game_date, players)VALUES('Colorado State', 45, 13, '20180831', ARRAY [1,2,3,4,5]),('Nebraska', 33, 28, '20180908', ARRAY [2,3,4,5,6]),('New Hampshire', 45, 14, '20180915', ARRAY [3,4,5,6,7]),('UCLA', 38, 16, '20180928', ARRAY [4,5,6,7,8]),('Arizona State', 28, 21, '20181006', ARRAY [5,6,7,8,9]),('Southern California', 20, 31, '20181013', ARRAY [6,7,8,9,10]),('Washington', 13, 27, '20181020', ARRAY [7,8,9,10,1]),('Oregon State', 34, 41, '20181027', ARRAY [8,9,10,1,2]),('Arizona', 34, 42, '20181102', ARRAY [9,10,1,2,3]),('Washington State', 7, 31, '20181110', ARRAY [10,1,2,3,4]),('Utah', 7, 30, '20181117', ARRAY [1,2,3,4,5]),('California', 21, 33, '20181124', ARRAY [2,3,4,5,6]);INSERT INTO football_players(name, year, major, passing_yards, rushing_yards, receiving_yards, img_src)VALUES('Cedric Vega', 'FSH', 'ARTS', 15, 25, 33, '../resources/img/player1.jpg'),('Myron Walters', 'SPH', 'CSCI', 32, 43, 52, '../resources/img/player2.jpg'),('Javier Washington', 'JNR', 'MATH', 1, 61, 45, '../resources/img/player3.jpg'),('Wade Farmer', 'SNR', 'ARTS', 14, 55, 12, '../resources/img/player4.jpg'),('Doyle Huff', 'FSH', 'CSCI', 23, 44, 92, '../resources/img/player5.jpg'),('Melba Pope', 'SPH', 'MATH', 13, 22, 45, '../resources/img/player6.jpg'),('Erick Graves', 'JNR', 'ARTS', 45, 78, 98, '../resources/img/player7.jpg' ),('Charles Porter', 'SNR', 'CSCI', 92, 102, 125, '../resources/img/player8.jpg'),('Rafael Boreous', 'JNR', 'MATH', 102, 111, 105, '../resources/img/player9.jpg'),('Jared Castillo', 'SNR', 'ARTS', 112, 113, 114, '../resources/img/player10.jpg');DROP TABLE favorite_colors;CREATE TABLE IF NOT EXISTS favorite_colors(  hex_value VARCHAR(6) PRIMARY KEY, /* This is the hexvalue for the color, it assumes that the value DOES NOT # */  name VARCHAR(50),                 /* The html safe name for the color.  This can be null */  color_msg  TEXT NOT NULL          /* A message describing the chosen color */);INSERT INTO favorite_colors(hex_value, name, color_msg)VALUES('FF6347', 'TOMATO', 'This color gets it name from the red fruit that at one time was considered poisonous!'),('3CB371', 'Medium Sea Green', 'Not sure what the difference is between Small &amp; Large Sea Green... but I guess this one is in between them.'),('EE82EE','Violet', 'Roses are Red, Violets are blue...'),('545AA7','Liberty', 'Not to be confused with the color of the Liberty Bell (which is indeed a copper color)');INSERT INTO favorite_colors(hex_value, color_msg)VALUES('FF2727', 'An unnamed red color'),('27FF27', 'An unnamed green color'),('870087', 'An unnamed magenta color'),('8F8FFF', 'An unnamed blue color');</code></pre>

 </dd>

 <dt>

  <ul>

   <li>Exit the psql terminal</li>

  </ul>

 </dt>

 <dd>

  <pre class="command-line" data-prompt="pick-unique-name-here::DATABASE="><code class="language-bash"> q</code></pre>

 </dd>

 <dt>

  <ul>

   <li>Head to your App’s Homepage</li>

  </ul>

 </dt>

 <dd>

  On your Heroku App’s Dashboard, click the “Open App” Button to open your App’s webpage in a new tab.

 </dd>

</dl>

<img decoding="async" alt="Screenshot of Heroku Resource Page" data-src="img/postgres_resource.png" class="img-fluid lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

<noscript>

 <img decoding="async" class="img-fluid" src="img/postgres_resource.png" alt="Screenshot of Heroku Resource Page">

</noscript>

To create a PostgreSQL database, you’ll need to first add a new Heroku Resource. Select the Heroku Resource tab and type in “postgres” to find the Heroku Postgres Resource.

<p class="alignleft h5">3. Submission Guidelines

<button class="btn btn-primary btn-sm alignbtn" type="button">Mark Complete</button> <button class="btn btn-primary btn-sm alignbtn" type="button" data-toggle="collapse" data-target="#multiCollapseExample4" aria-expanded="false" aria-controls="multiCollapseExample4">Expand</button>

<dl>

 <dt>

  <ul>

   <li>Create a link to your Heroku App</li>

  </ul>

 </dt>

 <dd>

  In a text file (lab_10_link.txt), write down the following:




  <ol>

   <li>Your name</li>

   <li>You partner’s name (if you have one)</li>

   <li>The link to your Heroku App</li>

  </ol>

 </dd>

 <dt></dt>

</dl>

<p class="h4 text-center">

<hr>