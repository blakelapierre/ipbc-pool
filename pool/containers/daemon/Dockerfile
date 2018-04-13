FROM blakelapierre/ipbc-base

VOLUME daemon-data

CMD cd ipbc/build/src && ./ipbcd --data-dir /daemon-data --rpc-bind-port 11898 --rpc-bind-ip 0.0.0.0 --confirm-external-bind