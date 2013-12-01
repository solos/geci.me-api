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
        "result": [
            { "aid": 2848529, "lrc": "http://s.geci.me/lrc/344/34435/3443588.lrc", "sid": 3443588, "artist_id": 2, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2346662, "lrc": "http://s.geci.me/lrc/274/27442/2744281.lrc", "sid": 2744281, "artist_id": 2396, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1889264, "lrc": "http://s.geci.me/lrc/210/21070/2107014.lrc", "sid": 2107014, "artist_id": 8715, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2075717, "lrc": "http://s.geci.me/lrc/236/23651/2365157.lrc", "sid": 2365157, "artist_id": 8715, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1563419, "lrc": "http://s.geci.me/lrc/166/16685/1668536.lrc", "sid": 1668536, "artist_id": 9208, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1567586, "lrc": "http://s.geci.me/lrc/167/16739/1673997.lrc", "sid": 1673997, "artist_id": 9208, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1571906, "lrc": "http://s.geci.me/lrc/167/16796/1679605.lrc", "sid": 1679605, "artist_id": 9208, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1573814, "lrc": "http://s.geci.me/lrc/168/16819/1681961.lrc", "sid": 1681961, "artist_id": 9208, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1656038, "lrc": "http://s.geci.me/lrc/179/17907/1790768.lrc", "sid": 1790768, "artist_id": 9208, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1718741, "lrc": "http://s.geci.me/lrc/187/18757/1875769.lrc", "sid": 1875769, "artist_id": 9208, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2003267, "lrc": "http://s.geci.me/lrc/226/22642/2264296.lrc", "sid": 2264296, "artist_id": 9208, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2020610, "lrc": "http://s.geci.me/lrc/228/22889/2288967.lrc", "sid": 2288967, "artist_id": 9208, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2051678, "lrc": "http://s.geci.me/lrc/233/23323/2332322.lrc", "sid": 2332322, "artist_id": 9208, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2412704, "lrc": "http://s.geci.me/lrc/283/28376/2837689.lrc", "sid": 2837689, "artist_id": 9208, "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2607041, "lrc": "http://s.geci.me/lrc/311/31116/3111659.lrc", "sid": 3111659, "artist_id": 9208, "song": "\u6d77\u9614\u5929\u7a7a" }
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
        "count": 16, 
        "code": 0, 
        "result": [
            { "aid": 1563419, "artist_id": 9208, "sid": 1668536, "lrc": "http://s.geci.me/lrc/166/16685/1668536.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1567586, "artist_id": 9208, "sid": 1673997, "lrc": "http://s.geci.me/lrc/167/16739/1673997.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1567586, "artist_id": 9208, "sid": 1673998, "lrc": "http://s.geci.me/lrc/167/16739/1673998.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1571906, "artist_id": 9208, "sid": 1679605, "lrc": "http://s.geci.me/lrc/167/16796/1679605.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1573814, "artist_id": 9208, "sid": 1681961, "lrc": "http://s.geci.me/lrc/168/16819/1681961.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1656038, "artist_id": 9208, "sid": 1790768, "lrc": "http://s.geci.me/lrc/179/17907/1790768.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 1718741, "artist_id": 9208, "sid": 1875769, "lrc": "http://s.geci.me/lrc/187/18757/1875769.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2003267, "artist_id": 9208, "sid": 2264296, "lrc": "http://s.geci.me/lrc/226/22642/2264296.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2020610, "artist_id": 9208, "sid": 2288967, "lrc": "http://s.geci.me/lrc/228/22889/2288967.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2051678, "artist_id": 9208, "sid": 2332322, "lrc": "http://s.geci.me/lrc/233/23323/2332322.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2412704, "artist_id": 9208, "sid": 2837689, "lrc": "http://s.geci.me/lrc/283/28376/2837689.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2607041, "artist_id": 9208, "sid": 3111659, "lrc": "http://s.geci.me/lrc/311/31116/3111659.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2647055, "artist_id": 9208, "sid": 3166350, "lrc": "http://s.geci.me/lrc/316/31663/3166350.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 2657468, "artist_id": 9208, "sid": 3180339, "lrc": "http://s.geci.me/lrc/318/31803/3180339.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 3093833, "artist_id": 9208, "sid": 3774083, "lrc": "http://s.geci.me/lrc/377/37740/3774083.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }, 
            { "aid": 3161846, "artist_id": 9208, "sid": 3861244, "lrc": "http://s.geci.me/lrc/386/38612/3861244.lrc", "song": "\u6d77\u9614\u5929\u7a7a" }
        ]
    }

根据歌手编号获取歌手信息(暂时只有歌手名)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+ 请求地址

  ``http://geci.me/api/artist/:artist_id``

+ 返回格式

    JSON

+ 请求方法

    GET

+ 示例
    
::

    curl 'http://geci.me/api/artist/9208' 

::

    {
        "count": 1, 
        "code": 0, 
        "result": {
            "profile": " ", 
            "name": "Beyond", 
            "area": "", 
            "alias": " ", 
            "birthday": "", 
            "constellation": ""
        }
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

    {
        "count": 1, 
        "code": 0, 
        "result": {
            "lrc": "http://s.geci.me/lrc/386/38612/3861244.lrc", 
            "sid": "3861244"
        }
    }

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

    {
        "count": 1, 
        "code": 0, 
        "result": {
            "cover": "http://s.geci.me/album-cover/157/1573814.jpg", 
            "thumb": "http://s.geci.me/album-cover/157/1573814-thumb.jpg"
        }
    }


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

