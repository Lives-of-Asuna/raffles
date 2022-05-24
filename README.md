# Lives of Asuna Raffle

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

**5-23-22:**

Seed drawn. https://etherscan.io/tx/0xe0877200d2c966ba0dc579bb5bf091c3ab3daa3d68149eca5f4169610ddb2cdd#statechange

Seed value: 70177777071533993175965106129838423495986341010648032094018797229518059778526

Total number of Asunas: 10000

Index of winning Asuna: 70177777071533993175965106129838423495986341010648032094018797229518059778526 % 10000 = 8526

Asuna ID at index 8526: [8526](https://opensea.io/assets/ethereum/0xaf615b61448691fc3e4c61ae4f015d6e77b6cca8/8526)

Holder of Asuna 8526 at the time of the snapshot: 0xe48c9423046d888AdA50501Cb4F5fC7754Bb8a81

**5-24-22:** 

Seed drawn. https://etherscan.io/tx/0x12625b33aa95362bdd3bab001bd3328408078850e6a6d53c41e27e1d48b99144#statechange

Seed value: 68506475599637254621240008595044904351200343545739017706036578325693045047392

Total number of Asunas: 10000

Index of winning Asuna: 68506475599637254621240008595044904351200343545739017706036578325693045047392 % 10000 = 7392

Asuna ID at index 7392: [7392](https://opensea.io/assets/ethereum/0xaf615b61448691fc3e4c61ae4f015d6e77b6cca8/7392)

Holder of Asuna 7392 at the time of the snapshot: 0x1a592B3F0A551D7F43CA03d83Fc4884Bf18C15f2


