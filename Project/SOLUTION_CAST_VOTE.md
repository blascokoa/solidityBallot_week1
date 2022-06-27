* Structure scripts to:
  * Deploy
  * Query proposals
  * Give vote right passing an address as input
  * Cast a vote to a ballot passing contract address and proposal as input and using the wallet in environment
  * Delegate my vote passing user address as input and using the wallet in environment
  * Query voting result and print to console

<hr />

<h3>Cast a vote to a ballot passing contract address and proposal as input and using the wallet in environment</h3>

  * 1st argument - proposal index: 1 (proposal "arg2")
  * Note that if an address has voted it cannot delegate voting right (``require(!sender.voted, "You already voted.)``)
  * Execute voting using function ``vote(uint256 proposal)``
  * Successfully voted for the 1st proposal ("arg2") with index 1
  * Transaction hash: ``0xf466f328fbd4cd8f8e1b68a638005af8650db75c5dc94c1c51d5bae061c34ae7``
```
yarn run ts-node --files ./scripts/Ballot/castVote.ts "1"

```
<img src="./castVote.png" alt="cast vote image"/>