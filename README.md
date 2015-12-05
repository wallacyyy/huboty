# Hubot-coffeepoll
[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard) [![Build Status](https://travis-ci.org/wallacyyy/hubot-coffeepoll.svg)](https://travis-ci.org/wallacyyy/hubot-coffeepoll) [![npm version](https://badge.fury.io/js/hubot-coffeepoll.svg)](http://badge.fury.io/js/hubot-coffeepoll) 

Hubot-coffeepoll is a Hubot plugin that helps your team to decide where to drink a coffee.
The hubot will search for coffee shops nearby and show options to people in the chat vote.

## Configuration

### Foursquare

You need to register at [Foursquare](https://developer.foursquare.com/) and set your credentials on this environment variables:

```
FOURSQUARE_CLIENT_ID = xxx
FOURSQUARE_CLIENT_SECRET = xxx
```

### Install

Install the plugin:

```
npm install hubot-coffeepoll --save
```

And add it to your ```external-scripts.json``` file:

```
[
  ...
  "hubot-coffeepoll"
  ...
]
```

## Usage 

### Configuring the place for next polls
```
hubot coffeepoll near <text>
```
Examples:
```
hubot coffeepoll near Champs-Elysées
hubot coffeepoll near my street
```
![](http://ditrospecta.com/images/2015-10-03-hubot-plugin/plugin-near-gif.gif)
### Starting the poll
```
hubot coffeepoll start 
```
![](http://ditrospecta.com/images/2015-10-03-hubot-plugin/plugin-start-gif.gif)
### Voting
```
hubot coffeepoll vote <number>
```
![](http://ditrospecta.com/images/2015-10-03-hubot-plugin/plugin-vote-gif.gif)
### Showing the partial results
```
hubot coffeepoll partial
```
![](http://ditrospecta.com/images/2015-10-03-hubot-plugin/plugin-partial-gif.gif)
### Finishing the poll and announcing the winner
```
hubot coffeepoll finish
```
![](http://ditrospecta.com/images/2015-10-03-hubot-plugin/plugin-finish-gif.gif)
