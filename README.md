# FabriccaliperSample

## Install
npm install -g --only=prod @hyperledger/caliper-cli@0.2.0
caliper bind --caliper-bind-sut fabric --caliper-bind-sdk 1.4.1   --caliper-bind-cwd ./ --caliper-bind-args=-g

## Run
byfn.sh start
caliper benchmark run --caliper-benchconfig myAssetBenchmark.json --caliper-networkconfig config.json --caliper-workspace ./ --caliper-flow-only-test --caliper-fabric-usegateway --caliper-fabric-discovery
