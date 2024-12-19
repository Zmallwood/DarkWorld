all: build_server

build_server:
	cd server; \
	cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=1 -B ../../build/server; \
	cmake --build ../../build/server --parallel 4;

run:
	cd ../build/server;\
	screen -d -m ./DarkWorldServer;
	xdg-open ./client/src/index.html;
	screen -r

