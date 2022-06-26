* Structure scripts to:
  * Deploy
  * Query proposals
  * Give vote right passing an address as input
  * Cast a vote to a ballot passing contract address and proposal as input and using the wallet in environment
  * Delegate my vote passing user address as input and using the wallet in environment
  * Query voting result and print to console

<hr />

<h3>Query voting result and print to console</h3>

  * Query winning proposal index (function ``winningProposal()``) and name (function ``winnerName()``)
  * ``winningProposal()`` returns index(type: BigNumber), converted into number 
  * ``winnerName()`` returns byte32 data, converted into string using ``ethers.utils.parseBytes32String()``

```
yarn run ts-node --files ./scripts/Ballot/QueryVotingResult.ts 

```
<img src="./queryResult.png" alt="query result image"/>