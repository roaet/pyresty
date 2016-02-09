#pyresty

`pyresty` is a requests wrapper inspired by [micha/resty](http://github.com/micha/resty). It provides a simple, concice shell interface for interacting with REST
services. 

##Quick Start

Install pyresty however you desire. I recommend `pip`.

```
$ pip install pyresty
```

Add a host to the configuration (ad-hoc hosts to be added soon):

```
$ pyresty add localhost http://localhost:8000/v2.0
```

Make requests:

```
$ GET /things
{[{"id": 1, "name": "superwidget"}, {"id": 2, "name": "not_cool_widget"}]}

$ DELETE /things/1
```

##Upcoming Features:

* ad-hoc host definition: `pyresty http://random.com`
* session recording and playback
* token loading from environment
* auth plugins
* host sections with more options
