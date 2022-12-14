# 이용 수수료

## 이용 수수료

WEMIX.Fi의 브릿지 이용 수수료는 사용자가 블록체인 네트워크 간에 토큰을 이동할 때 Multichain에 지불하는 비용입니다. 이용 수수료는 사용자가 이동하고자 하는 자산에서 자동으로 차감되며, 다음과 같이 계산됩니다.

| 구분                     | 이용 수수료                   |
| ---------------------- | ------------------------ |
| 기본 수수료                 | 이동 자산의 0.1%              |
| 브릿지 이용을 위한 최대/최소 수수료   | $5 \~ $1,000 가치의 토큰      |
| 브릿지 이용을 위한 최대/최소 토큰 수량 | $10 \~ $5,000,000 가치의 토큰 |

기본적으로 Multichain 브릿지의 이용 수수료는 이동하는 자산의 0.1%로 계산됩니다. 사용자가 이동하고자 하는 자산의 0.1%가 브릿지 이용을 위한 '최소 수수료'보다 작을 경우, 이용 수수료는 '최소 수수료'로 계산됩니다. 또한, 이동하고자 하는 자산의 0.1%가 '최대 수수료'보다 클 경우, 이용 수수료는 '최대 수수료'로 계산됩니다. 브릿지 이용을 위한 최대/최소 수수료는 메인넷에 따라 상이하며, 자세한 내용은 [브릿지: 수수료 지불 예시](fees.md#undefined)를 통해 확인할 수 있습니다. 이때, Multichain 브릿지를 통해 한 번에 이동할 수 있는 토큰의 수량은 최소 $10 에서 최대 $5,000,000 범위를 벗어날 수 없습니다.

| From 체인 | To 체인 | 자산의 종류        | 최대/최소 수수료                              | 최대/최소 토큰 수량                           |
| ------- | ----- | ------------- | -------------------------------------- | ------------------------------------- |
| 비트코인    | 위믹스   | BTC           | $0.9 / $1.9 BTC                        | $12 / $2천만 BTC                        |
| 이더리움    | 위믹스   | USDC          | $0.9 / $1.9 USDC                       | $12 / $2천만 USDC                       |
|         |       | WEMIX         | $5 / $1,000 WEMIX                      | $10 / $5백만 WEMIX                      |
| 클레이튼    | 위믹스   | KLAY          | $5 / $1,000 KLAY                       | $10 / $5백만 KLAY                       |
|         |       | WEMIX Classic | <p>$5 / $1,000</p><p>WEMIX Classic</p> | <p>$10 / $5백만</p><p>WEMIX Classic</p> |
| 위믹스     | 비트코인  | BTC           | $0.9 / $1.9 BTC                        | $12 / $2천만 BTC                        |
|         | 이더리움  | USDC          | $40 / $1,000 USDC                      | $50 / $2백만 USDC                       |
|         |       | WEMIX         | $80 / $1,000 WEMIX                     | $90 / $5백만 WEMIX                      |
|         | 클레이튼  | KLAY          | $5 / $1,000 KLAY                       | $10 / $5백만 KLAY                       |
|         |       | WEMIX         | $5 / $1,000 WEMIX                      | $10 / $5백만 WEMIX                      |

단, 사용자가 이더리움 메인넷으로 자산을 이동할 경우 브릿지 이용을 위한 최대/최소 수수료는 $80 \~ $1,000이며, 브릿지 이용을 위한 최대/최소 토큰 수량은 $90 \~ $5,000,000입니다.

{% hint style="info" %}
WEMIX.Fi의 브릿지 이용 수수료는 Multichain의 수수료 정책을 따르며, [Multichain Fees](https://docs.multichain.org/getting-started/fees)에서 확인할 수 있습니다.
{% endhint %}

## 수수료 지불 예시

### **이더리움, 클레이튼 메인넷에서 위믹스 메인넷으로 옮기는 경우**

철수는 이더리움 메인넷에서 100 USDC를, 클레이튼 메인넷에서 100 KLAY를 보유하고 있습니다. 위믹스 생태계에 참여하기 위해 자산을 옮기고 싶은 철수는 브릿지를 통해 자산을 옮기고자 합니다. 이때 철수는 이더리움 메인넷의 USDC를 옮기기 위해 수수료 0.9 USDC를 지불하고 클레이튼 메인넷의 KLAY를 옮기기 위해 수수료 1 KLAY를 지불하였습니다.

### **위믹스 메인넷에서 이더리움 메인넷으로 옮기는 경우**

영희는 위믹스 메인넷에서 100 USDC를 보유하고 있습니다. 위믹스 메인넷에서 다시 이더리움으로 자산을 옮기고 싶은 영희는 브릿지를 통해 자산을 옮기고자 합니다. 이때 위믹스 메인넷에서 이더리움으로 USDC를 옮기는 경우 최소 수수료가 다른 경우보다 높기 때문에 영희는 100 USDC보다 많은 양을 옮겨야 수수료를 낭비하지 않을 수 있습니다.

## 가스비

브릿지를 통해 토큰을 이동하기 위해 가스비가 별도로 필요합니다. 메인넷마다 부과되는 가스비가 다르며, 가스비를 지불하기 위한 WEMIX 코인이 부족할 경우 정상적인 실행이 어려울 수 있으니 사전에 확인할 것을 권장합니다. 메인넷 별 가스비는 가스 트래커 혹은 블록 탐색기를 통해 확인할 수 있습니다. 블록체인별 예상 가스비는 다음과 같습니다.

| 메인넷  | 예상 가스비                      | 가스 트래커                                                                                                           |
| ---- | --------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 이더리움 | 0.003647417870370370 ETH    | [https://etherscan.io/gastracker](https://etherscan.io/gastracker)                                               |
| 클레이튼 | 0.00038354894337000293 KLAY | [https://docs.klaytn.com/klaytn/design/transaction-fees](https://docs.klaytn.com/klaytn/design/transaction-fees) |
| 위믹스  | 0.0000001 WEMIX(=100GWEI)   | [https://explorer.wemix.com](https://explorer.wemix.com)                                                         |
