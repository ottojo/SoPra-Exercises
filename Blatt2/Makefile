all: domänenmodell.pdf
	$(info ARTIFACTS:domänenmodell.pdf)

domänenmodell.pdf: domänenmodell.dot
	dot -T pdf -o $@ domänenmodell.dot
