# Capsule House Raffle

This repository provides a history of the Lives of Asuna Legendary Raffle system.

Each Asuna is equivalent to one entry.

# Implementation Details

Prior to the drawing, a list of all qualified addresses with their corresponding Asuna IDs will be posted here, as well as the list of Asuna IDs.

On the day of the drawing, we will use `requestRandomWords` on https://etherscan.io/address/0x24c1e2873ec070011c09f15ded9b6f494470352f to generate a Chainlink VRF random seed. For example, let's say there are five Capsules eligible for the raffle, with the ids:

```
17
52
283
591
5183
```

Let's say Chainlink returns `87314876641541055251095431619250856243264627284949971051498783260561907368646` as our random seed.

To get the index of the winner, we do `87314876641541055251095431619250856243264627284949971051498783260561907368646 % 5 = 1`

The Asuna at index 1 is 52, so the owner of Asuna 52 wins at the time of the snapshot.

# Drawing History


