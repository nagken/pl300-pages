# Extra PL-300 concepts

Deeper-dive concepts beyond the basics.

## Storage modes deep-dive

Import: data into VertiPaq engine, fastest queries. DirectQuery: every interaction queries source. Dual: a table can act as Import for some joins and DQ for others. Live: thin connection to remote semantic model.

## Composite models

Mix Import + DirectQuery tables. Useful for joining a small high-perf dim (Import) to a huge DQ fact.

## Incremental refresh

Refresh only recent partitions; configure RangeStart/RangeEnd parameters in Power Query.

## Query folding tests

Right-click step -> 'View Native Query' available means it folds.

## DAX filter context

Filters from slicers, rows, columns, visual interactions - determine measure scope.

## Row context

Per-row context when iterating (in calculated columns and inside iterators).

## XMLA endpoint

Premium/PPU expose dataset for external tools (Tabular Editor, DAX Studio).

## Sensitivity labels

Apply Microsoft Purview labels to artifacts (auto-protect on export).
