

### schema : 

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract MyContract {
    // Code goes here
}

- `SPDX-License-Identifier`: Declares license.

- `pragma solidity ^0.8.0;`: Compiler version. Always required.

- `contract`: Defines a new contract (like a class).


### variables : 

- uint : positive intgeres

**just check the files in the website .**


### data location specifier : 

| Keyword    | Lifetime           | Mutable? | Gas Cost        | Used for                             |
| ---------- | ------------------ | -------- | --------------- | ------------------------------------ |
| `memory`   | Temporary          | Yes      | Medium          | Local vars, function arguments       |
| `storage`  | Persistent (state) | Yes      | High (on-chain) | State variables                      |
| `calldata` | Temporary          | No       | Low             | External function inputs (read-only) |

### global var : 

#### msg : 
|Property|Description|
|---|---|
|`msg.sender`|Address that **called the function**|
|`msg.value`|Amount of **Ether sent** with the call (in wei)|
|`msg.data`|Complete calldata (input bytes) of the call|
|`msg.sig`|First 4 bytes of the calldata (function selector)|