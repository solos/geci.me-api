.. Geci.me API documentation master file, created by
   sphinx-quickstart on Sun May 13 20:02:44 2012.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

歌词迷API文档
=======================================


.. toctree::
   :maxdepth: 2

Lyric
________

Get lyric by song
~~~~~~~~~~~~~~~~~~~~~

+ Resource url
  ``http://geci.me/api/lyric/:song``
+ Format
    JSON
+ Method
    GET
+ Example

::

    curl 'http://geci.me/api/lyric/海阔天空' 

::
    
    [
        {"aid": 1563419, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1668536}, 
        {"aid": 1571906, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1679605}, 
        {"aid": 1573814, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1681961}, 
        {"aid": 1618733, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u5468\u534e\u5065", "sid": 1740790}, 
        {"aid": 1656038, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1790768}, 
        {"aid": 1718741, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1875769}, 
        {"aid": 1889264, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u8d39\u7fd4", "sid": 2107014}, 
        {"aid": 2003267, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 2264296}, 
        {"aid": 2020610, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 2288967}, 
        {"aid": 2051678, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 2332322}, 
        {"aid": 2075717, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u8d39\u7fd4", "sid": 2365157}, 
        {"aid": 2253359, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u9ec4\u79cb\u751f", "sid": 2612812}, 
        {"aid": 2319680, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u4efb\u8d24\u9f50", "sid": 2705565}, 
        {"aid": 2346662, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u6797\u5b50\u7965", "sid": 2744281}, 
        {"aid": 2412272, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "DJ Tommy", "sid": 2837015}, 
        {"aid": 2412704, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 2837689}, 
        {"aid": 2497277, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u4fe1\u4e50\u56e2", "sid": 2957177}, 
        {"aid": 2600390, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u9ec4\u601d\u5a77", "sid": 3102406}, 
        {"aid": 2607041, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3111659}, 
        {"aid": 2647055, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3166350}, 
        {"aid": 2657468, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3180339}, 
        {"aid": 2740034, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u9648\u5609\u7490", "sid": 3296181}, 
        {"aid": 2771255, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u5f20\u60e0\u59b9", "sid": 3338621}, 
        {"aid": 2848529, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u7fa4\u661f", "sid": 3443588}, 
        {"aid": 2924795, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u5f20\u60e0\u59b9", "sid": 3548181}, 
        {"aid": 3093833, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3774083}, 
        {"aid": 3161846, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3861244}, 
        {"aid": 3289097, "song": "\u6d77\u9614\u5929\u7a7a", "artist": "\u9ec4\u601d\u5a77", "sid": 4028886}
    ] 


Get lyric by song and artist
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+ Resource url
  ``http://geci.me/api/lyric/:song/:artist``
+ Format
    JSON
+ Method
    GET
+ Example
    
::

    curl 'http://geci.me/api/lyric/海阔天空/Beyond' 

::

    [
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1668536, "aid": 1563419}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1679605, "aid": 1571906}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1681961, "aid": 1573814}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1790768, "aid": 1656038}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1875769, "aid": 1718741}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 2264296, "aid": 2003267}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 2288967, "aid": 2020610}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 2332322, "aid": 2051678}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 2837689, "aid": 2412704}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3111659, "aid": 2607041}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3166350, "aid": 2647055}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3180339, "aid": 2657468}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3774083, "aid": 3093833}, 
        {"song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3861244, "aid": 3161846}
    ]


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

