
default:	build

clean:
	rm -rf Makefile objs

build:
	$(MAKE) -f objs/Makefile

install:
	$(MAKE) -f objs/Makefile install

modules:
	$(MAKE) -f objs/Makefile modules

upgrade:
	/home/sumikum7/QUIC/nginx-1.16.1/sbin/nginx -t

	kill -USR2 `cat /home/sumikum7/QUIC/nginx-1.16.1/logs/nginx.pid`
	sleep 1
	test -f /home/sumikum7/QUIC/nginx-1.16.1/logs/nginx.pid.oldbin

	kill -QUIT `cat /home/sumikum7/QUIC/nginx-1.16.1/logs/nginx.pid.oldbin`
