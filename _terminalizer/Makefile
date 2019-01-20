%.yml:
	cwd=${PWD}
	cd ~ && \
	bash -c 'trap "" EXIT; terminalizer record demo -c ${PWD}/config.yml'; \
	mv demo.yml ${PWD}/$@

%.gif: %.yml
	terminalizer render $< -o $@

install-init: install-init.gif
