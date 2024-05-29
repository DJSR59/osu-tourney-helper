# osu! Tournament Helper Introductory Doc

This is the osu! Tournament Helper! The purpose of this project is to provide a web application service that will make it easier for hosts, staff members, and players to manage their tournaments. The end goal is to replace the system using Google Sheets or proprietary software so that users can have a generic, default system for running and playing in tournaments.

To start out, the project will not act as a replacement yet, but rather a tool for staff members and players to keep track, manage, and even have a easily look up system of tournaments. As progress continues, more and more aspects of tournaments will be accounted for until a vast majority of tournaments can be played solely using this system. This, of course, is with consideration of those using either vastly unique styles, or only parts of the application.

If you would like to contribute to this project by providing any feedback, testing, or even just keeping track of the project, follow this project's GitHub for more info. You can also contact me either using Discord _curlyq or in game CurlyQ.

## Table of Contents
- [osu! Tournament Helper Introductory Doc](#osu-tournament-helper-introductory-doc)
  - [Table of Contents](#table-of-contents)
  - [Tournament Management](#tournament-management)
  - [Landing Page](#landing-page)
  - [Regristration](#regristration)
  - [Team Management](#team-management)
  - [Player Listing](#player-listing)
  - [Mappool Player View](#mappool-player-view)
  - [Pooling](#pooling)
  - [Mappool Testing](#mappool-testing)
  - [Replaying](#replaying)
  - [Scheduling](#scheduling)
  - [Reffing](#reffing)
  - [Results](#results)
  - [Bracket](#bracket)
  - [Login](#login)
  - [User Profiles](#user-profiles)
  - [Tournament Viewing](#tournament-viewing)
  - [Settings](#settings)
  - [Modularity](#modularity)

## Tournament Management

A listing of the tournaments that are being used in the system that a player can access to view and participate in. For any ongoing tournaments, users are able to access these through the tournament listing and register. For any tournaments in which their regristrations are closed or have ended, players can view their details, like mappools and results, etc. The listing can be filtered and sorted based on names, dates, and more. For each listing, the name, a visual, and a minute amount of information is provided to the player for context and visually pleasing searching.

## Landing Page

The landing page serves as a "home" page for each tournament. The page should consist of any necessary information that should be known up-front, have any links to external sites that the player should be aware about, and easily access any part of the tournament, like mappools, schedules, etc. Depending on a user's role in a tournament, they would have access to different tabs, like a tester having access to the mappool testing tab, thus giving access to that respective page.

## Regristration

Regristration consists of a few parts. When captains form their teams and are ready to register, they will go to the Regristration page from the Landing Page to register their team. They will select Player Regristration and input all of their teams' information (osu! names, Discord usernames, general availability time zone) and send their submission to the host. 

When free agents want to register, they can select Free Agent Regristration and input all of their necessary information. This includes their osu! name, Discord username, availability, and a comments section for any strengths or weaknesses they may have, or any additional information. Free agents may also have the option to request joining a team by contacting the captain and having them accept their request. Any declines will also be reflected and the free agent will be prevented to ask again to avoid spam.

When staff members want to register, they can select Staff Regristration, choose which role they may desire, and add any additional information the host or admins may need to know about.

Regristration must happen within a specific timeline specified by the host. The host has access to different settings of the form to make it catered towards their tourney, like setting BWS, adding a general availability option, set roles, etc. Notifications will be sent to all parties when changes or updates have been made regarding their regristration.

## Team Management

Teams can be managed through a few different scenarios. Captains can manage the players on their teams by editing their information, switching them out for a new player, or removing a player from their team. If a team is already established, and a new player wanted to join them, they could send a request to the captain to join their team. If accepted, the member is automatically placed on the team roster. If a captain were to leave their team, the captain must transfer their role to another player on their team.

Players themselves can view their team roster. With their permissions, they should only have the functionality to remove themselves from the team if need be.

Hosts and admins can also have the ability to manage teams and information within all of the teams that are participating. They can also manage any role changes (from team to staff or from captain to player) if necessary. Notification will be sent to all parties when changes or updates have been made regarding their team.

## Player Listing

The player listing page consists of every single player that is registered into the tournament. Each listing should show a player's osu! name, they're rank, and their team that they're registered for. When clicking on a player's name, it can access their osu! profile. Users can search, filter, and sort through the player listing based on certain criteria to efficiently find certain players.

A team view can be accessed as well to see all of the teams, captains, and players in a different view. Through this team view, teams can be searched, filtered, and sorted using a different but similar set of criteria.

The free agents will have their own view as well, as they include having a comments about any additional information people should know. Free agents should still be able to be viewed even after the regristration period.

## Mappool Player View

The Mappool Player View is what all of the teams will see when they are looking at the pools for the different stages. The page for players will consist of different stages, each one having it's own mappool. Each mappool will have their own slots (no mod, hidden, double time, etc.), or any custom mods that the host sets. Each slot has the adequate amount of information a map should have to tell the player what kind of map it is, including any comments or notes that were given by the staff members. Players can click on the name of each map to open the osu! beatmap page for that song. Players can also download a mappack of each stage's pool granted if any staff members add one.

Initially, all of the pools will be hidden to the players so that it shows that the staff still need to work on a pool. Once a pool is ready to be shown to the players, the staff should be able to press a button to release the pool and make it available.

## Pooling

The pooling page is only open to staff members and admins. There are a couple parts to the pooling process. First, staff members, or "suggestors", can submit different maps for different mods. Any kind of map can be suggested, no matter the star ranking or ranked status, as long as it have a map ID. Maps that are suggested can be voted for by different poolers or staff members. The vote can consist of whether the map and mod for it are accurate, and their reasoning behind the pick. Once an adequate amount of votes are in for a map (up to the discretion of the host) the host can take the suggestion and put it into a slot in the pool.

After the suggestion process for each map, the map is placed into the pool. The map can be moved to any of the slots on the pool, as well as removed from the pool entirely. If a map is moved to a slot in which already has a different map on it, a confirmation notice will appear making sure the host knows there's a map in that slot already. Once confirmed, it will replace the map that was on the slot originally.

The host should be able to set the size of each of these pools before the tournament is even open, setting up what mods and how many of each will be used. The host can also add any custom slots if applicable.

Once the pooling process is done, it can be submitted to the testers for them to test and give feedback on the pool.

## Mappool Testing

In the Mappool Testing page, testers can give feedback on the mappool by giving votes and writing comments. A listing of the mappool will be showed and votes and feedback will be shown for each map in the pool. Once an adequate amount of tests have been made, the hosts/poolers can then make any modifications to the pool. Once any modifications have been submitted to the testers, the cycle continues until all parties give the green light to give the pools to the replayers.

## Replaying

Once a pool has been created and tested, it's time for the mappool showcase stream to be set up. In the stream, those that have the Replayer role will be able to send submissions of each map. The host will pick the best replays for each slot and then utilize them for their stream.

The page for both the host and replayers will consist of the slots that give their basic information and their beatmap link, as well as a listing of any submissions that have been given to the application. The host will select all of the replays and confirm to use their selected listing to use for the stream. Once confirmed, the host will get a folder with all of the replays.

## Scheduling

Once a pool is out for the public and the stream has been made, players will be able to access the scheduling page. Here, the teams can see a listing of the schedules, who is playing against who, and any referees or commentators that are assisting with the match.

The teams will start off with default times at the beginning of the stage provided by the host or staff members. Each captain can send a time change request to the other team if they wish to do so. The other team can accept, decline, or offer a different time to the other team. Once both teams accept a new time, that is reflected on the page and that will be the new time for the teams. If teams cannot come to a decision on a schedule, a forfeit option is available as well.

Hosts or staff members can set up default schedules when setting up the schedules page. If no default schedule is set, then the teams must choose a schedule themselves or a forfeit is drawn. Hosts can also manage these times in case of any extenuating circumstances, like forcing a forfeit on a team and such.

In order for referees, commentators, or streamers to be listed on a match, they must sign up for it. They can do so by going to the match ID and selecting the option to sign up, along with what role they're signing up for (for those that have multiple roles).

## Reffing

When matches begin to play, the referee is going to need some page in order to keep track of the match itself. It's going to have a decent amount of information, so the goal is to make it approachable and have a low learning curve.

Before the matches even start, the referee has to input what match ID they are reffing for. Once they do, the information will autofill with who to ping in Discord, who to invite to the match in game, the mappool, the team members, any score multipliers, and any other settings that are necessary before the match starts. Once the referee creates the lobby, they can also insert the MP link into the page.

If a team does not enter the lobby within the given amount of leeway time, the referee can set a forfeit for the one team, making the other team win by default. This will be reflected in both the Results and the Bracket page.

Once the page is ready and captains enter the lobby, if there is a pick/ban order phase, the page will reflect that the referee must do this first before moving on to the bans. If there are bans for this stage/tournament, the referee must pick the bans from both teams in whatever order is set. Once those have been input into the page, the referee can move on with the picks. Commands will be offered to the referee in which they can easily copy and paste them into the chat for them to use (mod settings, map, timer, etc.).

As the match goes underway, for each point each team takes the referee must reflect that onto the page. Once a team reaches the required amount of points to win, the page will reflect that.

Once the match is over, the referee has one final step, and that is to post/update the results, in which the results of this match are filled into the database for the results to properly render the results accurately. Once that is finished, the referee should be taken to the match selection screen.

## Results

Once matches are starting to be completed, creating the results page is next for the staff members. There are multiple ways to show results:

Solo Leaderboards for each map
Team Leaderboards for each map
Solo Placement Scores
Team Placement Scores
Match Costs/Individual Statistics
Pool Statistics

Using [this sheet](https://docs.google.com/spreadsheets/d/1YxqF-CDz2nN3rCbrcLdSW3uTkWOEG-yaA1t534c2aOk/edit#gid=1237373495) as a reference. If there are any other ways to show results that could be implemented, that can be talked about in the future, but these seem to be the most used views.

Hosts can set different views depending on which they prefer, and as the teams play, the information gets autofilled onto the results screen. Once all of the matches have been played, the results should automatically fill out the accurate information for the stage onto the results screen, in which the host can set different views that should be available to the public. Once set, the results screen can be public to the teams.

## Bracket

The Bracket page is supposed to replace using a Challonge bracket and make it more catered to osu! tournament hosts and creators. The bracket can have a few different modes:

Common team vs. team (both single and double elimination)
Round robin
Knockout lobby
And more...

For each mode the page can set how many teams/players there are, how many stages there are, and any other information that is necessary. The layout for each team listing should have their name, a team photo if applicable, and a score if the team has played yet or not.

The bracket should be modified and updated only if the results of each match is posted or if the host or admins manually enter them in.

## Login

Users must log in to use the web application. It's necessary since the application requires roles in order to access a majority of the features of the program. Logging into the application will only require a person's osu! login.

If a person is not logged in and attempts to use the system, the user will not be able to use the site until they do log in. Either that, OR the user can only access viewing other tournaments with a Guest account.

## User Profiles

User profiles show a good representation of who the player is and what tournaments they have played in. On the page shows the user's name itself as well as any contact information. There's also a listing of all the tournaments a user has been a part of, as well as any badges they may have. In the future, maybe also add items like a user's ETX or other bot ratings, BWS, or any other information that may be necessary for a tournament.

## Tournament Viewing

Tournament viewing allows users to look at other tournaments information and how the tournaments turned out. With a viewer role in the tournament, users can only see the mappools, schedules, and results in a finished state. They are unable to change, add, or modify anything about the tournament.

Users can search through a listing of tournaments that have been entered in the database. Any of the tournaments that the user has been a part of the user can also see, but the role must be reflected for each tournament.

## Settings

Application-global used settings page for those that want accessibility or notification adjustments. Self-explanatory, but requirements for this specifically will be better fleshed out later.

## Modularity

There's a good chance not everyone will like to do certain things on the web application. Maybe a good amount of players don't trust using a web application instead of using Google Sheets, or maybe the staff members don't want to learn the new system. There should be functionality to account for this. Possibly like some sort of importing and exporting functionality that will allow the host to easily input information from the application to any Google Sheets, and vice versa.

If there are any parts of the tournament process that are not being used (like streaming or team regristration), the application can be modular about this and be able to work with or without some parts. There are some parts that are integral, like pooling/testing, player registration, etc., but not every part is necessary and is up to customization.