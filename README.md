# Running a Replica node

This repo is setup to easily run inEVM replica nodes. Simply run `docker-compose up` to bring a replica node up locally.

The docker image for inEVM is hosted in a public docker repo: `offchainlabs/nitro-node:v3.5.2-33d30c0`

The nodeConfig file is prepopulated with inEVM parameters. The current setup uses a public rpc url for the Ethereum mainnet rpc and stores node data in docker volume.

The docker-compose is set up to use Arbitrum's public endpoints.

Set the flags `--parent-chain.connection.url` and `--node.data-availability.parent-chain-node-url` to your Arbitrum rpc provider of choice in order to speed up syncing.
