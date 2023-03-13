REPO_NAME=gobot
REPO_VER=dev

print:

dep-git:
	git clone git@github.com:hybridgroup/gobot.git -b $(REPO_VER)

dep-brew:
	# for video
	brew install mplayer

	# for joy stick.
	brew install sdl2

EX_FSPATH=$(PWD)/$(REPO_NAME)/examples


sys-nats-start:
	nats-server -js

run-video:
	cd $(EX_FSPATH) && go run tello_video.go
	