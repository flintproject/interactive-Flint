.PHONY: all clean

all: doc.zip

clean:
	-rm -rf doc doc.zip

doc:
	install -d $@

doc/rtm0.phml: | doc
	install -m 644 rtm0.phml doc/

doc/rtm1.phml: | doc
	install -m 644 rtm1.phml doc/

doc/example.pdf: | doc
	install -m 644 example.pdf doc/

doc.zip: doc/rtm0.phml doc/rtm1.phml doc/example.pdf
	zip -r doc doc
