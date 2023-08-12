# Created following tutorial https://github.com/Cyfrin/foundry-full-course-f23

## Useful commands:

`history -c` - clear terminal history
`source .env` - load env

`cast send {CONTRACT_ADDRESS} "store(uint256)" 57 --rpc-url $RPC_URL --private-key $PRIVATE_KEY`
    - call store func (write)
`cast call {CONTRACT_ADDRESS} "retrieve()"` - call view func (read)
`cast --to-base {hex-value} dec` - hex to decimal

`forge init` - init project
`anvil` - run local test blockchain
`forge fmt` - autoformat contracts
`forge script script/DeploySimpleStorage.s.sol --rpc-url $SEPOLIA_RPC_URL --private-key $PRIVATE_KEY --broadcast` - 
    deploy contract (without --broadcast it will simulate deploy)

`forge test --match-test {testFuncName}` - run specific test
`chisel` - execute solidity code in terminal line by line
`forge snapshot --match-test {testFuncName}` - save a snapshot of Function gas usage
`forge inspect FundMe storageLayout` - report of a contract vars

`cast storage {contractAddress}` - gives storage report from Etherscan (not working on Anvil)

`chainlist.org` - website contains info about chainIds
