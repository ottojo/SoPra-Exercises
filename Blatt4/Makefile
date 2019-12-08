all: client.pdf server.pdf
	$(info ARTIFACTS:client.pdf,server.pdf)

%.pdf: %.dot
	dot -T pdf -o $@ $<

.PHONY: clean
clean:
	rm client.pdf
