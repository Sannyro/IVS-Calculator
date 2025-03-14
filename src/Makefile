CC = gcc
CFLAGS = -g -std=c11 -Wall -Wextra -Werror -pedantic

BUILD_DIR := ./build
TEAM = xkadanm00_xhanzlj00_xklodom00

.PHONY: all pack clean test doc run stddev

all:

pack: clean
	cd .. && \
	mkdir $(TEAM) && \
	mkdir $(TEAM)/repo && \
	mkdir $(TEAM)/doc && \
	mkdir $(TEAM)/install && \
	find ./ -path ./$(TEAM) -prune -o -type f -exec cp --parents {} $(TEAM)/repo/ \; && \
	# add copy for doc and  && \
	cd $(TEAM) && \
	zip -r ../$(TEAM).zip * && \
	cd .. && \
	rm -rf $(TEAM)

clean:
	rm -f $(BUILD_DIR)/*
	rm -rf ../$(TEAM)
	rm -f ../$(TEAM).zip

test:

doc:
	doxygen Doxyfile

run:


stddev:
