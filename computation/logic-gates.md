## Logic gates

- [Logic gates](#logic-gates)
  - [And gate](#and-gate)
    - [Symbol](#symbol)
    - [Description](#description)
    - [Truth table](#truth-table)
  - [Or gate](#or-gate)
    - [Symbol](#symbol-1)
    - [Description](#description-1)
    - [Truth table](#truth-table-1)
  - [Not gate](#not-gate)
    - [Symbol](#symbol-2)
    - [Description](#description-2)
    - [Truth table](#truth-table-2)
  - [Nand gate](#nand-gate)
    - [Construction](#construction)
    - [Symbol](#symbol-3)
    - [Description](#description-3)
    - [Truth table](#truth-table-3)

### And gate

#### Symbol
![An and gate](../assets/and-gate.svg)

#### Description
-   This gate outputs `true` only if all the inputs are `true` and `false` otherwise
-   Takes two or more inputs

#### Truth table

| Input 1 | Input 2 | Output |
| ------- | ------- | ------ |
| True    | True    | True   |
| True    | False   | False  |
| False   | True    | False  |
| False   | False   | False  |


### Or gate

#### Symbol
![An or gate](../assets/or-gate.svg)

#### Description
-   This gate outputs `true` if atleast one of it's input is true and `false` otherwise
-   Takes two or more inputs

#### Truth table

| Input 1 | Input 2 | Output |
| ------- | ------- | ------ |
| True    | True    | True   |
| True    | False   | True   |
| False   | True    | True   |
| False   | False   | False  |


### Not gate

#### Symbol
![A not gate](../assets/not-gate.svg)

#### Description
-   Also known as the **inverter**
-   This gate changes the input to it's opposite
-   Takes one input

#### Truth table

| Input | Output |
| ----- | ------ |
| True  | False  |
| False | True   |


### Nand gate

#### Construction
![Construction of a nand gate](../assets/nand-gate-construction.svg)

#### Symbol
![A nand gate](../assets/nand-gate.svg)

#### Description
-   It is constructed by placing a `not` gate directly on the output of an `and` gate
-   Naming: Not+And = Nand
-   This gate outputs `false` only if all the inputs are `true` and otherwise `true`
-   Takes two or more inputs

#### Truth table

| Input 1 | Input 2 | Output |
| ------- | ------- | ------ |
| True    | True    | False  |
| True    | False   | True   |
| False   | True    | True   |
| False   | False   | True   |

