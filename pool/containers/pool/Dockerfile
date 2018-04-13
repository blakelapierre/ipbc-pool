FROM node:0.10.48

RUN apt-get update && apt-get install -y git build-essential cmake pkg-config libboost-all-dev libssl-dev libunbound-dev

RUN git clone https://github.com/blakelapierre/ipbc-pool

RUN cd ipbc-pool/pool && npm update

EXPOSE 8117
EXPOSE 3333

ADD config.json /ipbc-pool/pool/config.json

CMD cd ipbc-pool/pool && node init.js