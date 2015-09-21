# Syncing content across Drupal websites. 

## This is work in progress v.0.0.0! 
- don't expect this to work for you if you try install it on your Drupal site - it's probably really broken


### Rationale
There are plenty ways to do this - and I've dabbled in a few of them:

 - node export
 - deploy
 - feeds
 - services and rest server. 


This is my simplified take on it based on the requirements of the current project. 

The source site keeps a register of destination subsciber sites, and pings each with a notification that content has 
been insered or changed. Part of the payload of that notification is a URI where the full content can be downloaded via 
a Services module REST server endpoint. 

It is up to the destination server to fetch and import the content. 


- 2 modules - 1 for Source, 1 for destinations
- Content types should be configured the same on each Source and Destination

More detail to follow


