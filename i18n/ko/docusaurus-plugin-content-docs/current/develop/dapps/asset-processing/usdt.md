import Button from '@site/src/components/button'

# USDT Processing

## Tether

스테이블코인은 가격을 안정적으로 유지하기 위해 법정 화폐나 금과 같은 자산에 1:1로 고정된 암호화폐의 일종입니다. 최근까지 jUSDT 토큰이 있었는데, 이는 [bridge.ton.org](bridge.ton.org)를 통해 이더리움 토큰을 브릿지한 ERC-20 기반의 래핑된 토큰입니다. 하지만 [2023년 4월 18일](https://t.me/toncoin/824), [Tether](https://tether.to/en/)사가 발행한 **네이티브** USD₮ 토큰의 공개 출시가 있었습니다. USD₮가 출시된 후 jUSDT는 우선순위가 두 번째로 밀렸지만 여전히 USD₮의 대안 또는 추가 수단으로 서비스에서 사용되고 있습니다.

In TON Blockchain USD₮ supported as a [Jetton Asset](/develop/dapps/asset-processing/jettons).

:::info
To integrate Tether’s USD₮ Token on TON Blockchain use the contract address:
[EQCxE6mUtQJKFnGfaROTKOt1lZbDiiX1kCixRv7Nw2Id_sDs](https://tonviewer.com/EQCxE6mUtQJKFnGfaROTKOt1lZbDiiX1kCixRv7Nw2Id_sDs?section=jetton)
:::

<Button href="https://github.com/ton-community/assets-sdk" colorType="primary" sizeType={'sm'}>Assets SDK</Button>
<Button href="https://docs.ton.org/develop/dapps/asset-processing/jettons" colorType={'secondary'} sizeType={'sm'}>Jetton Processing</Button>
<Button href="https://github.com/ton-community/tma-usdt-payments-demo?tab=readme-ov-file#tma-usdt-payments-demo" colorType={'secondary'} sizeType={'sm'}>TMA USDT payments demo</Button>

## Advantages of USD₮ on TON

### Seamless Telegram integration

[USD₮ on TON](https://ton.org/borderless) will be seamlessly integrated into Telegram, offering a uniquely user-friendly experience that positions TON as the most convenient blockchain for USDt transactions. This integration will simplify DeFi for Telegram users, making it more accessible and understandable.

### Lower transaction fees

Fee consumed by Ethereum USD₮ transfer is calculated dynamically depending on the network load. That's why transaction can cost a lot.

```cpp
transaction_fee = gas_used * gas_price
```

- `gas_used` is the amount of gas was used during transaction execution.
- `gas_price` price on 1 unit of gas in Gwei, calculated dynamically

On the other hand average fee for sending any amount of USD₮ in TON Blockchain is about 0.0145 TON nowadays. Even if TON price increases 100 times, transactions will [remain ultra-cheap](/develop/smart-contracts/fees#average-transaction-cost). The core TON development team has optimized Tether’s smart contract to make it three times cheaper than any other Jetton.

### Faster and scalable

TON’s high throughput and rapid confirmation times enable USD₮ transactions to be processed more quickly than ever before.

## Advanced Details

:::caution IMPORTANT

See important [recommendations](/develop/dapps/asset-processing/jettons#jetton-wallet-processing).
:::

## See Also

- [Payments Processing](/develop/dapps/asset-processing/)
