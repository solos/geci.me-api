.. Geci.me API documentation master file, created by
   sphinx-quickstart on Sun May 13 20:02:44 2012.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

歌词迷API文档
=======================================


.. toctree::
   :maxdepth: 2

歌词
________

根据歌曲名获取歌词
~~~~~~~~~~~~~~~~~~~~~

+ 请求地址

  ``http://geci.me/api/lyric/:song``

+ 返回格式

    JSON

+ 请求方法

    GET

+ 示例

::

    curl 'http://geci.me/api/lyric/海阔天空' 

::

    {
        "count": 15, 
        "code": 0, 
        "result": 
            [
                {"aid": 1563419, "lrc": "http://s.geci.me/lrc/166/16685/1668536.lrc", "artist": "Beyond", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 1668536}, 
                {"aid": 1571906, "lrc": "http://s.geci.me/lrc/167/16796/1679605.lrc", "artist": "Beyond", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 1679605}, 
                {"aid": 1573814, "lrc": "http://s.geci.me/lrc/168/16819/1681961.lrc", "artist": "Beyond", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 1681961}, 
                {"aid": 1618733, "lrc": "http://s.geci.me/lrc/174/17407/1740790.lrc", "artist": "\u5468\u534e\u5065", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 1740790},
                {"aid": 1656038, "lrc": "http://s.geci.me/lrc/179/17907/1790768.lrc", "artist": "Beyond", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 1790768},
                {"aid": 1718741, "lrc": "http://s.geci.me/lrc/187/18757/1875769.lrc", "artist": "Beyond", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 1875769},
                {"aid": 1889264, "lrc": "http://s.geci.me/lrc/210/21070/2107014.lrc", "artist": "\u8d39\u7fd4", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 2107014},
                {"aid": 2003267, "lrc": "http://s.geci.me/lrc/226/22642/2264296.lrc", "artist": "Beyond", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 2264296},
                {"aid": 2020610, "lrc": "http://s.geci.me/lrc/228/22889/2288967.lrc", "artist": "Beyond", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 2288967},
                {"aid": 2051678, "lrc": "http://s.geci.me/lrc/233/23323/2332322.lrc", "artist": "Beyond", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 2332322},
                {"aid": 2075717, "lrc": "http://s.geci.me/lrc/236/23651/2365157.lrc", "artist": "\u8d39\u7fd4", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 2365157},
                {"aid": 2253359, "lrc": "http://s.geci.me/lrc/261/26128/2612812.lrc", "artist": "\u9ec4\u79cb\u751f", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 2612812},
                {"aid": 2319680, "lrc": "http://s.geci.me/lrc/270/27055/2705565.lrc", "artist": "\u4efb\u8d24\u9f50", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 2705565},
                {"aid": 2346662, "lrc": "http://s.geci.me/lrc/274/27442/2744281.lrc", "artist": "\u6797\u5b50\u7965", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 2744281},
                {"aid": 2412272, "lrc": "http://s.geci.me/lrc/283/28370/2837015.lrc", "artist": "DJ Tommy", "song": "\u6d77\u9614\u5929\u7a7a", "sid": 2837015}
            ]
    }


根据歌曲名和歌手名获取歌词
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+ 请求地址

  ``http://geci.me/api/lyric/:song/:artist``

+ 返回格式

    JSON

+ 请求方法

    GET

+ 示例
    
::

    curl 'http://geci.me/api/lyric/海阔天空/Beyond' 

::
    
    {
        "count": 14, 
        "code": 0, 
        "result": 
            [
                {"lrc": "http://s.geci.me/lrc/166/16685/1668536.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1668536, "aid": 1563419}, 
                {"lrc": "http://s.geci.me/lrc/167/16796/1679605.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1679605, "aid": 1571906}, 
                {"lrc": "http://s.geci.me/lrc/168/16819/1681961.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1681961, "aid": 1573814}, 
                {"lrc": "http://s.geci.me/lrc/179/17907/1790768.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1790768, "aid": 1656038}, 
                {"lrc": "http://s.geci.me/lrc/187/18757/1875769.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 1875769, "aid": 1718741}, 
                {"lrc": "http://s.geci.me/lrc/226/22642/2264296.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 2264296, "aid": 2003267}, 
                {"lrc": "http://s.geci.me/lrc/228/22889/2288967.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 2288967, "aid": 2020610}, 
                {"lrc": "http://s.geci.me/lrc/233/23323/2332322.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 2332322, "aid": 2051678}, 
                {"lrc": "http://s.geci.me/lrc/283/28376/2837689.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 2837689, "aid": 2412704}, 
                {"lrc": "http://s.geci.me/lrc/311/31116/3111659.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3111659, "aid": 2607041}, 
                {"lrc": "http://s.geci.me/lrc/316/31663/3166350.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3166350, "aid": 2647055}, 
                {"lrc": "http://s.geci.me/lrc/318/31803/3180339.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3180339, "aid": 2657468}, 
                {"lrc": "http://s.geci.me/lrc/377/37740/3774083.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3774083, "aid": 3093833}, 
                {"lrc": "http://s.geci.me/lrc/386/38612/3861244.lrc", "song": "\u6d77\u9614\u5929\u7a7a", "artist": "Beyond", "sid": 3861244, "aid": 3161846}
            ]
    }

根据歌曲编号获取歌词URL
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+ 请求地址

  ``http://geci.me/api/lrc/:song_id``

+ 返回格式

    JSON

+ 请求方法

    GET

+ 示例
    
::

    curl 'http://geci.me/api/lrc/3861244' 

::

    { "count": 1, "code": 0, "result": {"lrc": "http://s.geci.me/lrc/386/38612/3861244.lrc"} }

根据专辑编号获取专辑封面URL
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+ 请求地址

  ``http://geci.me/api/cover/:album_id``

+ 返回格式

    JSON

+ 请求方法

    GET

+ 示例
    
::

    curl 'http://geci.me/api/cover/1573814' 

::

    { "count": 1, "code": 0, "result": {"cover": "http://s.geci.me/album-cover/157/1573814.jpg", "thumb": "http://s.geci.me/album-cover/157/1573814-thumb.jpg"} }



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

