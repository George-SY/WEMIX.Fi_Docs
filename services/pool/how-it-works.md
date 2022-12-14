# 동작원리

## 유동성 풀

WEMIX.Fi의 유동성 풀은 AMM을 통해 사용자가 코인과 토큰을 교환할 수 있는 스마트 컨트랙트입니다. 풀 컨트랙트가 생성되면 토큰 쌍이 공급되면서 형성된 교환 비율에 따라 거래가 체결됩니다. 풀의 유동성이 적을수록 토큰 쌍의 교환 비율은 크게 변하며, Slippage 및 Price Impact로 인한 피해가 발생할 수 있습니다. 사용자의 피해를 최소화하고 안정적인 거래를 지원하기 위해 풍부한 유동성을 확보하는 것은 필수 조건입니다.

WEMIX.Fi는 풀의 초기 유동성을 제공하고 더 많은 거래를 활성화하기 위해 사용자의 참여를 독려합니다. 사용자가 풀에 유동성을 직접 공급하면, 공급한 유동량에 따라 스왑 수수료의 일부를 얻을 수 있습니다. 스왑 사용자가 토큰을 교환할 때 지불한 수수료(자산의 0.25%)의 일부가 유동성을 제공한 사용자의 지분에 따라 분배되며, 많은 유동량을 공급한 사용자일수록 더 많은 수익을 얻을 수 있습니다. 풀의 총 유동성에 대한 사용자의 지분은 LP 토큰으로 증명할 수 있습니다.

WEMIX.Fi의 유동성 풀을 구성하는 토큰 쌍의 가치는 1:1로 유지됩니다. 비율이 1:1에서 벗어날 경우 차익거래의 기회가 생기며 스왑이 활발하게 이루어지면 통해 다시 1:1로 회복됩니다. 유동성을 안정적으로 유지하고 과도한 차익거래가 발생하는 것을 방지하기 위해 사용자가 공급하는 유동성은 1:1 비율로 예치됩니다. 사용자가 예치할 수량을 직접 입력하여 토큰 쌍의 비율이 다를 경우, 더 많은 가치를 가진 토큰이 일부 스왑되어 풀에 예치됩니다.

{% hint style="info" %}
사용자와 유동성 풀 사이에 토큰의 거래가 이루어지는 과정과 Slippage 및 Price Impact에 대한 자세한 내용은 [스왑: 동작원리](../swap/how-it-works.md)에서 확인할 수 있습니다.
{% endhint %}

## 비영구적 손실&#x20;

비영구적 손실이란 자산의 가격이 급격하게 변할 때 유동성 풀에 예치된 자산의 가치가 예치하지 않았을 때의 가치보다 낮아지면서 발생하는 손실을 의미합니다. 사용자는 풀에 예치한 자산의 지분에 따라 수익을 얻을 수 있지만, 자산의 가격이 급격하게 변할 경우 유동성 풀의 특징에 따라 손실이 발생할 수 있습니다. 예를 들어:

* WEMIX의 가격이 $100이고 WEMIX$의 가격이 $1 일 때, 사용자가 WEMIX-WEMIX$ 풀에 10 WEMIX와 1,000 WEMIX$를 예치하여 총 $2,000 가치의 유동성을 제공하고 전체 유동성의 10% 지분을 확보했습니다.
* 얼마 뒤, WEMIX의 가격이 $100에서 $150으로 급격하게 올랐고 스왑 사용자들의 차익거래를 통해 WEMIX의 수량은 감소하고 WEMIX$의 수량은 증가했습니다. 풀을 구성하는 토큰 쌍의 수량이 각각 81.65 WEMIX와 12,247 WEMIX$로 총 $24,494.50의 가치가 유동성이 남게 되었습니다. 이때 사용자가 출금을 신청할 경우, 10%의 지분으로 $2,449.50을 받을 수 있습니다.
* 만약, 사용자가 자산을 예치하지 않았다면 보유한 10 WEMIX와 1,000 WEMIX$의 가치는 $2,000에서 $2,500으로 올랐을 것이며, 사용자가 풀에서 출금한 $2,449.50 대비 약 $50(2.0%) 정도 손실된 금액입니다.

비영구적 손실은 가격의 변동이 클수록 더 크게 발생하며, 손실의 정도를 예측하기 어렵습니다. 또한, 시장 상황에 따라 손실이 다시 복구될 수 있기 때문에 사용자는 풀의 예상 수익률과 시장 상황을 면밀히 관찰할 필요가 있습니다. 가격의 변동에 따른 비영구적 손실은 다음과 같이 표현할 수 있습니다.

<figure><img src="../../.gitbook/assets/Impermanent Loss of CPMM Model.png" alt=""><figcaption><p>CPMM 모델의 비영구적 손실 그래프</p></figcaption></figure>

* 가격이 0.25배 상승할 경우, 0.6% 비영구적 손실 발생
* 가격이 0.5배 상승할 경우, 2.0% 비영구적 손실 발생
* 가격이 0.75배 상승할 경우, 3.8% 비영구적 손실 발생
* 가격이 1.0배 상승할 경우, 5.7% 비영구적 손실 발생
* 가격이 2.0배 상승할 경우, 13.4% 비영구적 손실 발생
* 가격이 3.0배 상승할 경우, 20.0% 비영구적 손실 발생
* 가격이 4.0배 상승할 경우, 25.5% 비영구적 손실 발생
