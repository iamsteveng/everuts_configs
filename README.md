## Combine all json files to single one file

```
jq -s . ./products/*.json > all_products.json
```

## Update Matching RAS config

Development

```
npx @offbeattech/dynamodb-data-loader --table "DevMatchingRasScheme" --path "matching/FR.json"
```

Test

```
npx @offbeattech/dynamodb-data-loader --table "TestMatchingRasScheme" --path "matching/FR.json"
```
