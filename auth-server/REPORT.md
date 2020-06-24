# OAuth Comparative Analysis

## OAuth Provider : SPOTIFY 

### Research Conducted By: Paul Depew

### Overall Score and Comments
#### Score (Out of 10): 8
#### General Comments
Spotify grants a variety of rights access depending on the scope given. Most of the rights are silo'd to Android of iOS requests and the only way to make a persistent token is to utilize one of those frameworks. 

#### Pros
* Simple to set up with great documentation
* Allows for streaming media between the connections

#### Cons
* Must generate custom base 64 challenge hashes
* Does not allow updated of the Spotify user from the Oauth
* Limited time, tough to persist

### Ratings and Reviews
#### Documentation
The documentation is very strong. It lays out the foundations from start to finish and provides samples and code examples. I wish they would make their urls a little more noticeable and is they put more descriptions behind their key needs. 

#### Systems Requirements
It can play with all places that need it, due to the nature of its calls. Heroku, Amazon... sky is the limit. The only real limitation is streaming rights vs web token authorization. For some reason not all rights are avialable to all systems. 

#### Ramp-Up Projections
This should take about an hour or two to create a connection and test to see which user rights you would prefer to use. Then depending on what requests to put to their api after, and how to deal with those objects. 

#### Community Support and Adoption levels
There is not an active community supporting this unfortunately as Spotify wants to keep their information proprietary to their platform and approved interactions. There are a few github projects trying to break it into a public api but they do not do streaming, only getting of information (like playlists, likes, most recent plays etc)


### Links and Resources
* [framework](https://developer.spotify.com/documentation/web-api/)
* [docs](https://developer.spotify.com/documentation/general/guides/authorization-guide/#authorization-code-flow-with-proof-key-for-code-exchange-pkce)
* [examples/tutorials](http://xyz.com)

### Code Demos
* [live/running application](http://xyz.com)
* [code repository](https://github.com/PaulDepew/oauth-server)

### Operating Instructions
If someone were to download your repo (above), what steps do they need to take to run the application
* `npm start`
* Endpoint: `/`
  * Returns a JSON object verifiying user data.
* Endpoint: `/oauth`
  * interfaces with spotify to provide oauth.