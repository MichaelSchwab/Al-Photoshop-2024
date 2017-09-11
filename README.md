# IOTA commandline wallet
A commandline based wallet for the IOTA crypto currency, based on nodejs

In order to run the wallet on an regular basis, consider to run your own IOTA full node,
how to do this is shown in the section "Setting up a IOTA full node" below.

Installation:

Install nodejs Version >= 8.0.0
create a directory and put the my-wallet.js and iota-wallet-config.js in there

install additional modules

`npm install iota.lib.js`

`npm install nedb`

Now you are ready to rum
enter
`node my-wallet.js help`

Introductional Video
https://www.youtube.com/watch?v=nWo1vwNsXfo

Setting up a IOTA full node, just a brief overview
1. Get access (or setup yourself) to a 64Bit Windows or Linux or Mac server which has a public IP or can be reached from the internet using something like DynDns
2. Be sure the server runs 24/7 and is intended to alwas be connected to the internet.
3. Install Oracle Java RuntimeEnvironment (JRE) 64Bit. You might download it from here http://www.oracle.com/technetwork/java/javase/downloads/server-jre8-downloads-2133154.html
4. Get the precompiled IOTA Reference Implementation (IRI) from here https://github.com/iotaledger/iri/releases. Download the precompiled jar. For example the iri-1.3.2.jar
5. Copy the iri to a directory where it can be executed in.
6. Write a startup script. Just one line is enough. Example: java -Xmx1G -jar iri-1.3.2.jar -c iri.ini --remote --remote-limit-api "removeNeighbors, addNeighbors, interruptAttachingToTangle, attachToTangle"
7. Get neighbours, therefore goto https://slack.iota.org/ and join the community and enter the channel nodesharing. On this cannel are more people like you searching for neighbours, just get in touch and find 4-9 Neighbours.
7. Edit iri.ini suit your needs.

A more detailed description can be found
[here] (https://forum.iota.org/t/setting-up-a-headless-node-on-a-ubuntu-iri-version-1-2-1/1332)
and
[here] (https://github.com/iotaledger/iri)


