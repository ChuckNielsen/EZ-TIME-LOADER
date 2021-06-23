# EZ-TIME-LOADER
Streamline your transit traveling experience by having content delivered on a GPS + timeline triggered event.

App = EZ TIME LOADER
Functionalities - EZ TIME MAP SCHEDULING
Route dictates music playlist 
Also dictates playlist length, meaning that we can insert any audio from any application as a commercial or ad from the app. Adding value to the experience of utilizing EZ TIME’s Map Scheduling, you won’t have to look down at your phone for updates or worry about new notifications while using other features of the phone such as full screen gaming or walking to and from destinations.
Notify access - *** feature*** gps triggered zones where alerts can go off leading up to an intersection so the user can decide to review notifications further or wait until a later time. We also do this when entering a bus for audo of the stop and how many stops up it is - alarm for stop arriving happens to both players of the 2 player game. Allowing for users the option to share the stop they are getting off or not. This adds the sense of community by localizing users with landmarks that signifies a users location. 
End users
People with headphones that travel on foot and transit (car feature / couples game - netflix movie decider can be played while at work or on break without the others needed input right away
Input and output process
Current process of steps from an end user perspective of clicks and events// 
1, open music app, 
2. Find music 
3 play music 
4 switch to maps app 
5 type location of destination 
6 use public transit and/or walk 
7, get to bus stop 
8, check phone / reply to messages, see bus wait time for arrival, 
9. Get on bus while listening to music 
10. Get alerted from maps app when to depart 
11. Arrive to destination and remove headphones 

7 times the user physically touches phone current trip

EZ TIME Apparatus
1. Open phone to ez time
2. Type destination and choose music genre / playlist of choice AND Choose 2 player game (tick tack toe, hangman, checkers, chess or couples movie picker) 
3. Put on headphones 
4. Walk to bus stop
5. Get alerted on arrival in low volume the wait time for arrival with new message count (new messages are muted while using application for deferred delivery of messages/notifications)
6. When bus arrives vol low again with bus stop name and time
7. Get alert on phone to pull stop 
8. Auto Pause game to get off bus
9. Finish game after exiting vehicle if needed, also get notification update alert on bus departure 
10. With music pausing at the destination (storefront) entrance and the option to continue listening. 


4 times to physically touch phone while using multiplayer ez rider functionality 
only 3 events if not (app inputs at start (3 inputs - address, playlist/genre and game to play on transit), notification (optional looks), game (optional) plays, continue playing music on arrival (optional)

Engineering teams

Dev ops - deployment of docker and kubernotes clusters on back end 

Mobile app deployment - 2 teams
1st team - front end UX/UI creation
2nd team - web app developers

Make web app that is hosted on a website and can be saved as a bookmarked shortcut on both android phone / iPhone
This app has the 
google maps api
Spotify api
Youtube api
Slack api (plus other messaging services but 1 for now)

After route is chosen with estimated travel time and arrival time to multiple locations until getting to end point we need to auto generate a music playlist based on genre and travel time then play it when beginning travel on foot.

The next feature will be using the phones gps to trigger events that are all predetermined upon opening application and typing destination
We know what music to play and when to pause it with updates of arrival times and delivered messages

We also know which matchmaking room to put the user in based on arrival time to stop (we are aiming at less than 60 seconds from arriving to location for the game to be loaded and both players playing (on both ends).

Plus the added ability to do matchmaking for 2 player games that last 1-10 minutes , tic tac toe, checkers, hangman, 
These games will be chosen when route is made and played upon arriving to stop with auto pause features of transit arrival notification.

By granting access to phones application privileges (google maps, spotify/youTUBE, messages, slack, facebook ++other social media platforms) we will be able to update our user of notifications after they are delivered in grouped bundles notified at decided gps points
“on site on scene” making it a safer experience while using mobile phones and communicating in public, safe zones to drop messages.
 

Need to figure out what the best options are for granting user privileges and the control a webpage api of Spotify grants the software. Can you use the phone application and control it in the background? Or would you have to log into Spotify on the mobile website to listen? Would this limit the ability to hear audio when the screen is locked?

Add tracing ability to allow dev ops to trace when a function is evoked in the app. This will be great for analytics of message retrieval and game wait times as well as completed games

Further reading - https://classroom.udacity.com/nanodegrees/nd064-1/parts/30cb07da-8fd4-4438-a209-b3457adb5d82/modules/7b21dfa4-aac8-4d24-82c5-65325e6dc691/lessons/fcc8c401-8331-4214-9609-f2f8529f50a1/concepts/eb97edd8-bc15-4c09-82b3-e45f71c34c3d

Health Checks - explore the core reasons to introduce health checks and implementations examples
Prometehus Best Practices on Metrics Naming - explore how to name, label, and define the type of metrics
Application Logging Best Practices - read more on how to define what logs should be collected by an application
Logging Levels - explore possible logging levels and when they should be enabled
Enabling Distributed Tracing for Microservices With Jaeger in Kubernetes - learn what tools can be used to implement tracing in a Kubernetes cluster
