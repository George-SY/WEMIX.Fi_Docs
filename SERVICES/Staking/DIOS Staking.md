# 디오스 스테이킹

디오스 스테이킹 프로그램에 예치하고 위믹스 공식 스테이블코인 WEMIX$ 가치 안정화에 참여하세요. WEMIX를 예치하고 WEMIX$의 성장과 함께 리워드를 획득할 수 있습니다.

* 예치 즉시 WEMIX$ 리워드가 지급됩니다.
* 리워드의 재예치를 통해 추가 리워드를 획득할 수 있습니다.
* 언제든 출금과 재예치가 가능합니다.

## 스테이블코인 WEMIX$ 가격 안정화

위믹스의 스테이블코인 WEMIX$는 USDC를 담보로 발행되어 USDC와 동일한 가치를 갖습니다. 위믹스는 WEMIX$의 가치가 USDC와 페깅되도록 안정화 프로토콜인 DIOS(Dollar In and Out Stabilizer)를 구축하였으며, 생태계의 상태에 따라 USDC와의 비율이 증가하거나 감소할 경우, 두 가지의 내부 프로토콜을 실행하여 원복하도록 설계되었습니다. 생태계가 성장함에 따라 WEMIX$의 가치가 USDC 보다 증가할 경우, TIP(Treasury In Protocol)가 실행되고 반대로 생태계가 축소함에 따라 WEMIX$의 가치가 USDC 보다 감소할 경우, TOP(Treasury Out Protocol)가 실행되어 WEMIX$의 가치를 안정적으로 유지합니다. 디오스 스테이킹 프로그램 참여자는 DIOS를 통해 발생한 수익의 일부를 얻을 수 있습니다.

### TIP(Treasury In Protocol)

생태계가 성장함에 따라 WEMIX$의 가치가 USDC보다 증가할 경우, **DIOS는 가치 안정화를 위해 WEMIX$를 발행**합니다. 이때, 1 WEMIX$는 1개 이상의 USDC와 교환되며, 교환된 USDC는 **Treasury와 스테이킹 프로그램에 분배**됩니다.

예를 들어, WEMIX$의 가치가 $1.5로 증가한 경우를 가정합니다. DIOS에서 발행된 1 WEMIX$는 1.5 USDC로 교환되며, Treasury와 스테이킹 프로그램에 각각 1 USDC와 0.5 USDC가 분배됩니다.

### TOP(Treasury Out Protocol)

생태계가 축소함에 따라 WEMIX$의 가치가 USDC보다 감소할 경우, **DIOS는 가치 안정화를 위해 Treasury에서 USDC를 출금**합니다. 이때, 1 USDC는 1개 이상의 WEMIX$와 교환되며, 교환된 **WEMIX$의 일부는 소각되고 나머지는 스테이킹 프로그램에 분배**됩니다.

예를 들어, WEMIX$의 가치가 $0.5로 감소한 경우를 가정합니다. Treasury에서 출금된 1 USDC는 2 WEMIX$로 교환되며, 1 WEMIX$는 소각하고 1 WEMIX$는 프로그램에 분배됩니다.

### 가스비&#x20;

TIP/TOP를 통해 안정화 작업을 하는 과정에서 거래가 발생하기 때문에 가스비가 발생합니다. 가격을 안정화 하는 과정에서 발생하는 수익의 0.1%는 이러한 가스비를 충당하기 위한 컨트랙트에 귀속되며, 나머지 99.9%는 디오스 스테이킹 예치자에게 리워드로 돌아갑니다.&#x20;

가스비 컨트랙트 주소: 0xCD656326947a94E0E65bc4Ad48142fFAe5732c10

## 포인트 정책

디오스 스테이킹 프로그램의 포인트 정책은 자산을 장기간 예치한 사용자에게 추가 혜택을 제공하는 정책으로, 사용자는 포인트 정책에 따라 자산을 장기간 예치할수록 더 높은 이자율을 얻을 수 있습니다. 사용자는 1년 예치 시 최대 100% 고정 APR에 대한 지급 포인트를 획득할 수 있으며, 지급 포인트는 1 포인트당 1 WEMIX의 가치를 갖는 가산 포인트로 전환할 수 있습니다. 전환된 가산 포인트는 사용자의 예치금에 합산되어 더 많은 리워드를 획득합니다.

### 지급 포인트

지급 포인트는 사용자가 1년 동안 자산을 예치했을때 추가로 획득할 수 있는 APR을 1초 단위로 보여주는 지표입니다. 예를 들어, 사용자가 1년 동안 1,000 WEMIX를 예치할 경우 지급 포인트 1,000 포인트를 획득할 수 있습니다. 누적된 지급 포인트를 가산 포인트로 전환하면 이자율이 가산되며, 정책에 따라 2,000 WEMIX를 예치한 것과 동일한 지급 리워드를 획득할 수 있습니다. 지급 포인트는 실시간으로 누적되며, WEMIX.Fi 'Portfolio' 메뉴의 '나의 Staking' 메뉴를 통해 확인할 수 있습니다.

### 가산 포인트

가산 포인트는 사용자가 획득한 지급 포인트가 1 WEMIX의 가치를 갖고 예치금에 합산되는 포인트입니다. 사용자는 'Portfolio' 메뉴의 '나의 Staking' 메뉴를 통해 지급 포인트를 가산 포인트로 전활 할 수 있습니다. 또한, 사용자가 자산을 추가로 예치하거나 리워드를 재예치할 경우 지급 포인트는 가산 포인트로 자동 전환됩니다.

가산 포인트는 사용자가 프로그램에서 출금하는 자산에 비례하여 소멸되며, 사용자는 출금 시 '소멸 예정 가산 포인트'를 확인할 수 있습니다. 예를 들어, 1,000 WEMIX를 6개월 동안 예치하여 가산 포인트 500 포인트를 획득한 경우, 300 WEMIX를 출금하면 150 (300/1,000 \* 500)의 가산 포인트가 소멸됩니다.

## **리워드 재예치**

리워드 재예치는 프로그램에서 발생한 리워드를 WEMIX로 교환한 뒤 다시 예치하는 기능입니다. 재예치 과정에서 지급 포인트는 가산 포인트로 자동 전환되며, 사용자는 손쉽게 복리 이자를 획득할 수 있습니다. 단, 리워드 재예치 시 WEMIX$를 WEMIX로 교환하는 과정에서 스왑 수수료가 발생합니다.
