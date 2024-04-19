# Solana Keypair Generator

This script generates a Solana Keypair using the `@solana/web3.js` library.

## Prerequisites

Before running the script, ensure you have Node.js installed on your machine.

## Installation

1. Clone this repository to your local machine.
2. Navigate to the directory where you cloned the repository.
3. Install the dependencies using the following command:

    ```bash
    npm install @solana/web3.js
    ```

## Usage

1. Open the JavaScript file where you want to generate the Keypair.
2. Add the following import statement at the top of your file:

    ```javascript
    import { Keypair } from "@solana/web3.js";
    ```

3. Generate a new Keypair by calling the `Keypair.generate()` function:

    ```javascript
    const keypair = Keypair.generate();
    ```

4. Access the public and secret keys of the generated Keypair:

    ```javascript
    console.log(`The public key is: `, keypair.publicKey.toBase58());
    console.log(`The secret key is: `, keypair.secretKey);
    ```

## Example

Here's an example script that generates a Keypair and logs its public and secret keys:

```javascript
import { Keypair } from "@solana/web3.js";

const keypair = Keypair.generate();

console.log(`The public key is: `, keypair.publicKey.toBase58());
console.log(`The secret key is: `, keypair.secretKey);

```

## RUN THE CODE 

``` node generateKeypair.js ```

## OUTPUT ![image](https://github.com/Solana0x/solanadev/assets/142747768/e106bee7-1204-44b2-802c-a3a184a42d39)
