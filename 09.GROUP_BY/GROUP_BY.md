## USE

- To group rows from a table based on one or more columns
- Helps with aggregate functions
- Summarizes information
- Aides in analysis of large data sets

_NOTE_ : _It is essential to select categorical or discrete columns_

### The GROUP BY Operation follows

- Split - Dataset is divided into groups based on unique values in the "Region" column
- Apply - Aggregate functions are applied to specified column within each region group
- Combine - combines the aggregated result

```ASCII
╭────────┬─────────┬─────────────╮          ╭───────┬──────╮
│ Region │ Product │ SalesAmount │    ╭────▶│ North │ 1000 │
├────────┼─────────┼─────────────┤    │     ├───────┼──────┤
│ North  │    A    │    1000     ├────┤     │ North │ 1200 │     ╭─────────┬──────╮
├────────┼─────────┼─────────────┤    │     ╰───────┴──────┴────▶│  North  │ 2200 │
│ South  │    A    │    1500     ├────┤                          ├─────────┼──────┤
├────────┼─────────┼─────────────┤    │     ╭───────┬──────┬────▶│  South  │ 3300 │
│ North  │    B    │    1200     ├────┤     │ South │ 1500 │     ╰─────────┴──────╯
├────────┼─────────┼─────────────┤    │     ├───────┼──────┤
│ South  │    B    │    1800     ├────┴────▶│ South │ 1800 │
╰────────┴─────────┴─────────────╯          ╰───────┴──────╯
```
