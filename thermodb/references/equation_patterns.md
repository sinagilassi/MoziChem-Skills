# Equation patterns

## Vapor pressure pattern

Source form:
`ln P = C1 + C2/T + C3 ln T + C4 T^C5`

Executable YAML form:

- map coefficients to `parms[...]`
- map variables to `args[...]`
- map result to `res[...]`
- use `math.log` and `math.exp`
- include explicit normalization lines for each coefficient, even if the divisor is `1`

## Heat-capacity polynomial pattern

Example source form:
`Cp/R = a0 + a1 T + a2 T^2 + a3 T^3 + a4 T^4`

Scaled headers such as `a1 × 10^3`, `a2 × 10^5`, `a3 × 10^8`, `a4 × 10^11` must be represented in `UNIT`, not `SYMBOL`.

## Extended blocks

Equation tables may include:

- `BODY`
- `BODY-INTEGRAL`
- `BODY-FIRST-DERIVATIVE`
- `BODY-SECOND-DERIVATIVE`

If the template or source supports them, keep all blocks.

## Special-case row pattern

If one compound uses a different equation from the rest of the table:

- add another `EQ-n`
- use an equation selector column according to project convention
- do not infer equation choice from missing coefficients alone
