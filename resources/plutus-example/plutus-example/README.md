# plutus-example

This library demonstates end to end examples of creating and executing Plutus scripts on chain.

This is done roughly in the following steps:

1. Write your Plutus **on chain** code.
2. Serialize your Plutus on chain code to the text envelope format (`cardano-cli` expects this format).
3. Create your transaction with the accompanying Plutus script(s).
4. Submit transaction to execute Plutus script.

## FAQ

### Where is the off chain code?

The off chain code is used for transaction construction. In this case we construct the transaction with `cardano-cli` and therefore we don't need to write any off chain code.

### Where can I learn about Plutus scripts in more detail?

Our education director, Lars Brünjes, has an excellent series of [tutorials](https://youtu.be/IEn6jUo-0vU) on youtube. We will not attempt to provide an indepth explanation of Plutus in this repository.

## Tutorials

We demonstate the following scripts:

1. Simple transaction output ["locking" Plutus script](plutus-example/plutus-example/src/Cardano/PlutusExample/LockingScript.hs) that always succeeds.
2. Simple minting Plutus script (In progress).

The `plutus-example` executable outputs a text envelope formatted txin locking plutus script that always succeeds.

More to come...

