demo/%.yml:
	cwd=${PWD}
	cd ~ && \
	bash -c 'trap "" EXIT; terminalizer record demo -c ${PWD}/config.yml'; \
	mv demo.yml ${PWD}/$@

demo/%.gif: demo/%.yml
	terminalizer render $< -o $@

install-init: demo/install-init.gif
install-update: demo/install-update.gif
