# 컨트랙트

## WEMIX.Fi와 브릿지를 통해 연결이 가능한 메인넷&#x20;

위믹스 메인넷과 다른 메인넷 간에 자산을 이동하기 위해서는 먼저 두 메인넷이 브릿지를 통해 연결이 가능한지 확인해야 합니다. 현재 WEMIX.Fi와 연결 가능한 메인넷은 다음과 같습니다. 다음 메인넷에 존재하는 자산을 위믹스 메인넷으로 옮기거나, 반대로 위믹스 메인넷에서 다른 메인넷으로 옮길 수 있습니다.

| Name     | Chain ID | Currency | Explorer                                                  | Public RPC Endpoint                                                                                  |
| -------- | -------- | -------- | --------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| Ethereum | 1        | ETH      | [https://etherscan.io](https://etherscan.io)              | [https://mainnet.infura.io/v3/](https://mainnet.infura.io/v3/)                                       |
| Klaytn   | 8217     | KLAY     | [https://scope.klaytn.com](https://scope.klaytn.com)      | [https://public-node-api.klaytnapi.com/v1/cypress](https://public-node-api.klaytnapi.com/v1/cypress) |
| WEMIX3.0 | 1111     | WEMIX    | [https://explorer.wemix.com](https://explorer.wemix.com/) | https://api.wemix.com                                                                                |

## WEMIX.Fi와 브릿지를 통해 이동이 가능한 토큰

현재 WEMIX.Fi에서 브릿지를 통해 이동 가능한 토큰은 다음과 같습니다. 서로 다른 메인넷에 존재하는 토큰은 각자 다른 컨트랙트로 존재하기 때문에 사용자는 반드시 이를 유의하여야 합니다.

| # | Name          | Token Address                              | Chain    |
| - | ------------- | ------------------------------------------ | -------- |
| 1 | BTC           |                                            | Bitcoin  |
| 2 | USDC          | 0x7EA2be2df7BA6E54B1A9C70676f668455E329d29 | Ethereum |
| 3 | WEMIX Classic | 0x2c69095d81305F1e3c6ed372336D407231624CEa | Ethereum |
| 4 | USDC          | -                                          | Klaytn   |
| 5 | WEMIX         | 0x2bf9b864cdc97b08b6d79ad4663e71b8ab65c45c | Klaytn   |
| 6 | USDC          | -                                          | WEMIX    |
| 7 | WEMIX         | -                                          | WEMIX    |
