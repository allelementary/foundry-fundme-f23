`history -c` - clear terminal history
`source .env` - load env

`cast send 0xCf7Ed3AccA5a467e9e704C703E8D87F634fB0Fc9 "store(uint256)" 57 --rpc-url $RPC_URL --private-key $PRIVATE_KEY`
    - call store func (write)
`cast call 0xCf7Ed3AccA5a467e9e704C703E8D87F634fB0Fc9 "retrieve()"` - call view func (read)
`cast --to-base {hex-value} dec` - hex to decimal

`forge init` - init project
`anvil` - run local test blockchain
`forge fmt` - autoformat contracts
`forge script script/DeploySimpleStorage.s.sol --rpc-url $SEPOLIA_RPC_URL --private-key $PRIVATE_KEY --broadcast` - 
    deploy contract (without --broadcast it will simulate deploy)
