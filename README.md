Graille-Labs - Screeper Project - JsonApi bundle
=====================
**DEVELOPMENT IN PROGRESS**

![Screeper](http://img4.hostingpics.net/pics/8388841405135647.png)

The JsonApi bundle add support of JsonApi (alecgorge's plugin) in symfony 2.

The github of JsonApi : https://github.com/alecgorge/jsonapi

The webpage of JsonApi : Not available

Installation
------------
Add :

```
"graille-labs/screeper-jsonapi-bundle": "dev-master"
```

in your composer.json

Configuration
------------
You must configure servers in the ServerBundle :

ServerBundle Page : https://github.com/graille/ServerBundle

Usage
------------

For use, you must call the service :

```
$api = $this->container->get('screeper.json_api.services.api')->getApi("servername");
```

After that, you can use the api normally.
If "servername" is empty, the default server will be used (For more informations, go to the [ServerBundle](https://github.com/graille/ServerBundle) page).