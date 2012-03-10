


test: test.beam
	erlc test.erl

dist_demo: dist_demo.beam
	erlc dist_demo.beam

start: dist_demo
	erl -sname "Server" -s dist_demo start -s init stop

send_rpc: test
	erl -sname "Client" -s test send_rpc
