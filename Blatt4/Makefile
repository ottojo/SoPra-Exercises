all: client.pdf
	$(info ARTIFACTS:client.pdf)

client.pdf: client.dot
	dot -T pdf -o $@ client.dot

.PHONY: clean
clean:
	rm client.pdf
