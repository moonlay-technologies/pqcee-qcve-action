# QCVE - Code Scanning Example

This action analyze submitted CodeQL Query against Pre-defined Databases from public project, and return sarif report to folder

## Example usage

```
name: CodeQL Scan
id: scan
uses: maulanardy/codeql-sample-action@v1.2.0
with:
  username: 'john'
  report: '${{ github.workspace }}/output/john'
  query: '${{ github.workspace }}/queries/john'
  database: 'openssl'
  number: 1

```

## Inputs

- `username`: the name of the owner of the query.
- `report`: location of generated sarif report.
- `query`: location of submitted query.
- `database`: selected database to analyze.
- `number`: unique request number


## Available databases

- `openssl`: database languange `javascript`.
- `bitcoin`:  database languange `javascript`.
