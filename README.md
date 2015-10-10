feature:

	double click to run，don't need config，support rtmp and hls live

	
run and quit:

	double click bin/liveserver.bat to run，press ctrl-c to quit.
	
	
use:
	
	default：
	1、rtmp publish：rtmp://127.0.0.1/live/[streamname]
	2、rtmp play：rtmp://127.0.0.1/live/[streamname]
	3、hls play：http://127.0.0.1/hls/[streamname].m3u8
	4、live stat；http://127.0.0.1/stat
	custom：
	1、config file：/usr/local/nginx/conf/nginx.conf

	
Depand:
	
	1、use open source project：cygwin nginx nginx-rtmp-module
	2、nginx's configure param：--with-http_dav_module --with-http_flv_module --with-http_stub_status_module --without-http_scgi_module --without-http_uwsgi_module --without-http_gz ip_module --without-http_ssi_module --without-http_proxy_module --without-http_memcached_module --without-http_empty_gif_module --without-mail_pop3_module --without-mail_imap_module --without-mail_smtp_module --with-pcre=$PWD/../pcre-8.36 --add-module=$PWD/../nginx-rtmp-module-master


Why make it:

    I want a live server with one command or double click to run. 
    Rtmplite has the feature with pool compatibility. This liveserver
    with double click to run and needn't config. It has good 
    compatibility and support 64 clients. it's efficiency is poor 
    than linux server but enough for personal application.


Site:
	
	www.github.com/langsim/liveserver
