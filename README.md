# Ballot Solidity Contract
EncodeClub Bootcamp - Week 1

## Team Members
```
Francis_ldn#7100
Yerin#6129
Blasco#9303
ziii#4702
```

## Project work

> `castVote.ts` (ziii#4702)

Implemented the TS script for a given user to cast a vote on a certain proposal in one ballot.

1. Two command line arguments are passed into the script - `ballotAddress` and `proposal_num`, referring to the address of the smart contract `ballot` deployed on ropsten network and the number id of the proposal to vote, respectively
2. The (lack of) arguments are checked with error handling code
3. Connection to the deployed ballot smart contract is made with the current voter account
4. The `vote` function on the smart contract is invoked with the `proposal_num` argument.
5. Appropriate progress messages are logged on screen.

