


test: test.erl
	erlc test.erl

dist_demo: dist_demo.erl
	erlc dist_demo.erl

start: dist_demo
	erl -sname "Server" -s dist_demo start -s init stop

send_rpc: test
	erl -sname "Client" -s test send_rpc
