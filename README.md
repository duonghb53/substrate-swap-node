## Add ORML Pallets

Using ORML Pallets: orml-currencies, orml-tokens, orml-traits, orml-utilities

## Define an Exchange Protocol

The Exchange pallet defines a simple interface that depends on the ORML pallets that were configured
in the previous step:

- `submit_order(from_id, from_amt, to_id, to_amt)`
- `take_order(order_id)`
- `cancel_order(order_id)`
- `get_balance_token(id, currency_id)`

## Build & Run

If you need to,
[set up your Substrate development environment](https://substrate.dev/docs/en/knowledgebase/getting-started/#manual-installation).
Then, build and run a development chain:

```shell
$ cargo run -- --dev --tmp
```

Once the node is running, use this link to open the Polkadot JS Apps UI and connect to the Substrate
node: https://polkadot.js.org/apps/#/settings/developer?rpc=ws://127.0.0.1:9944. Use the Settings >
Developer app and the contents of the [`types.json`]) file to add the
necessary types to the UI.

## Upstream

This project was forked from the
[Substrate Developer Hub Node Template](https://github.com/substrate-developer-hub/substrate-node-template).
