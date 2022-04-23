# terra_firstDapp

making sure you are using node 16
```
nvm use 16
```


instantiating contract
```
- events:
    - type: from_contract
      attributes:
        - key: contract_address
          value: terra1jek2p9h9f75nkaf86t35z0vyqknsw7rxpq06jn
        - key: method
          value: instantiate
        - key: owner
          value: terra1nvfp6z70wqstzaflwst3gpydvx8p7kh0fzhy3l
        - key: count
          value: "0"
    - type: instantiate_contract
      attributes:
        - key: creator
          value: terra1nvfp6z70wqstzaflwst3gpydvx8p7kh0fzhy3l
        - key: admin
        - key: code_id
          value: "66361"
        - key: contract_address
          value: terra1jek2p9h9f75nkaf86t35z0vyqknsw7rxpq06jn
    - type: message
      attributes:
        - key: action
          value: /terra.wasm.v1beta1.MsgInstantiateContract
        - key: module
          value: wasm
        - key: sender
          value: terra1nvfp6z70wqstzaflwst3gpydvx8p7kh0fzhy3l
    - type: wasm
      attributes:
        - key: contract_address
          value: terra1jek2p9h9f75nkaf86t35z0vyqknsw7rxpq06jn
        - key: method
          value: instantiate
        - key: owner
          value: terra1nvfp6z70wqstzaflwst3gpydvx8p7kh0fzhy3l
        - key: count
          value: "0"
```

Interact with the deployed contract
```
$ terrain console --network testnet
terrain > await lib.increment(wallets.bombay);

  txhash: 'F76A165062849CD45A0B35E41692FD55E7C7DB442787BB21FD5F96583785491C',
  raw_log: '[{"events":[{"type":"execute_contract","attributes":[{"key":"sender","value":"terra1nvfp6z70wqstzaflwst3gpydvx8p7kh0fzhy3l"},{"key":"contract_address","value":"terra1jek2p9h9f75nkaf86t35z0vyqknsw7rxpq06jn"}]},{"type":"from_contract","attributes":[{"key":"contract_address","value":"terra1jek2p9h9f75nkaf86t35z0vyqknsw7rxpq06jn"},{"key":"method","value":"try_increment"}]},{"type":"message","attributes":[{"key":"action","value":"/terra.wasm.v1beta1.MsgExecuteContract"},{"key":"module","value":"wasm"},{"key":"sender","value":"terra1nvfp6z70wqstzaflwst3gpydvx8p7kh0fzhy3l"}]},{"type":"wasm","attributes":[{"key":"contract_address","value":"terra1jek2p9h9f75nkaf86t35z0vyqknsw7rxpq06jn"},{"key":"method","value":"try_increment"}]}]}]',
  gas_wanted: 160553,
  gas_used: 102039,
  height: 8749254,
  logs: [
    TxLog {
      msg_index: 0,
      log: '',
      events: [Array],
      eventsByType: [Object]
    }
  ],
  code: 0,
  codespace: '',
  data: '0A280A262F74657272612E7761736D2E763162657461312E4D736745786563757465436F6E7472616374',
  info: '',
  timestamp: ''
}
```

Front-end scaffolding


<img width="844" alt="image" src="https://user-images.githubusercontent.com/56182747/164893754-18bcf3f7-225a-46d9-9491-7abb31d0eb15.png">
