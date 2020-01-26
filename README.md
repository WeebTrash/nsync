This is meant to be a tool to sync your (the user) watched progress between plex, emby and jellyfin.
 
# Goals

- Recognize a user from the tokens we receive within the session e.g. you login into plex and jellyfin in the session, the client will connect the two accounts and retrieve the data
- figure out the watch differences between one service and another(plex<->jellyfin)
- link shows and movies via the agents to say tvdb ids
- catch events of watched things so it’s synced on all services
- save user+token in db 
 
 

# MVP
* Capability of adding slave states to master sum
* syncOut/figure out differences between master and specific slave(s)
* Matching TV shows and Movies between agents/servers
* TV/Movie data storage structure
* Generic show/movie database NAME TVID MOVIEDBID IMDBID TYPE
* Be able to sync JF and Plex to master

# TODO
* further API structs
* Master specific data per item: `internalID Progress`
* WebUI fetches year/poster/ratings/etc
* Think about how to grab data later on
* webUI with master and slave list
* Have a button to sync in from slaves and sync out to apply status from master to all (singular in future) server
* Future: events from any server update the others via master
* Edge case: think about how to seperare progress and singular watched episodes

