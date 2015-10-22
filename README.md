# Dexie Sync-server Tools
A library for creating Offline-First applications.

WARNING: BETA BETA, very much beta. Used internally at Spoddler but utilizing a public repo just for fun.

Let your app run in the browser and not require them to be online. Accomplished without sacrificing security. Users only sync what they are authorized to access.

# Use Cases
* Offline webapps in browsers, tablets or phones that require continous backup of the client-based database whenever being online.
* Offline-capable email- and calendar client.
* Collaboration with other users in common teams, groups or similar.

# Features
* [ISyncProtocol](https://github.com/dfahlander/Dexie.js/wiki/Dexie.Syncable.ISyncProtocol) instance to use with [Dexie.Syncable.js](https://github.com/dfahlander/Dexie.js/wiki/Dexie.Syncable.js)
* npm package to use from nodejs after having authenticated the sync request. Send client changelog and get server changelog back to user.

# It's required by you to:
* Setup your node/express server
* Define your SQL schema for you application model.
* Let each table have a column
* Access Control definitions: For each table, you define a property 
 
# Compared to Meteor
* Embraces relational model
* This is just a library to use from your nodejs based server application
* You authenticate your users in your own fashion. Dexres just needs a user-ID string.
* You define how access is controlled for your data.

# Compared to Couch/PouchDB
* Embraces relational model
* Access control your javascript objects so that they can be shared between users or teams, or dedicated to single users.
* This is just a library to use from your nodejs based server application
* You authenticate your users and you define access patterns for each table.

