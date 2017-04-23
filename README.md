
# antlr-parser

Parser for Ethereum's Solidity language generated by ANTLR4 and wrapped in RxJS.


## Installation

`npm i -S @solidity-ide/antlr-parser`


## Example

ts```
import { SolidityParser } from "SolidityParser";

const parser = new SolidityParser();

parser.Observable().subscribe(
    rule => console.log(rule.type),
);

parser.ErrorObservable().subscribe(
    e => console.log(e),
);

parser.parseFile("./voting.sol");
```
