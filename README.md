# Chainlink OpenSea External Adapter (WIP)

## Input Params

- `offset`, `startAt`: The # of contracts to offset
- `limit`, `qty`: Limit of contracts/dapps to return

## Output

```json
{
 "jobRunID": "278c97ffadb54a5bbb93cfec5f7b5503",
 "data": {
  ["collections": [..],
  "result": 250]
 },
 "statusCode": 200
}
```

## Install Locally

Install dependencies:

```bash
yarn
```

Natively run the application (defaults to port 8080):

### Run

```bash
yarn start
```

## Call the external adapter/API server

```bash
curl -X POST -H "content-type:application/json" "http://localhost:8080/" --data '{ "id": 0, "data": { "offset": "0", "limit": "1" } }'
```
