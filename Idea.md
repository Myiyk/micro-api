Universe API
============
Universe / Universal / Universary

Based on microservices and partial library.

Idea
====
Programmer can work only on Application, not backend.

Targets
-------
# Super easy API
# Super easy integration
# Completely modular system
# 100% open source
# Possible use of server code in browser
# Single requirements that is Node.js in serverside
# Maximal easy source code
# Minimal HW requirements (Raspberry should run full functionality server with response < 100ms)
# Security
# Easy to learn (self describe)

Second level targets
--------------------
# Use JavaScript
# Use minimal number of requirements
# Well documented 

Browser
    Application Code
    Library API
    Internal functions
    Internal storage / cache
    HTTP / Socket communication

API functions
-------------
Depends on installed modules, this is describe of all modules.

- Gateway
- Permission module
- Watchers
- Project container
- Key Value storage
- Queue storage
- Data object storage


Way of request
Internet -> Gateway -> Permission -> |Watchers| Project container / KV / Queue / Data

Arrows show visibility model, internal modules don't know about external.

Gateway works only with Permissions
Permissions works only with data services and watchers


Scenarios of using
-------------------
- User browsing eshop products in public internet
- Administrator of eshop adding new product
- User send message to other user

Security
--------
Complete api is disabled until unlock

var api = Api.init();
api.enable({port: 80});