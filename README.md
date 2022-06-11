# Adding Kujira Testnet to Keplr wallet

You can follow these steps in Google Chrome, Brave browser or any other browser which supports Keplr wallet extension.

## 1) Open Keplr wallet, right click on it and click on ``Inspect``.

This will open ``DevTools`` window.

![](https://www.synergynodes.com/images/kujira-testnet-keplr/Kujira-Testnet-Keplr-01-min.png)

## 2) On the ``DevTools`` window, click on ``Console`` tab.

![](https://www.synergynodes.com/images/kujira-testnet-keplr/Kujira-Testnet-Keplr-02-min.png)

## 3) Copy the following code.

```
window.keplr.experimentalSuggestChain({
    chainId: "harpoon-4",
    chainName: "Kujira Testnet",
    rpc: "https://rpc.kujira.pupmos.network",
    rest: "https://api.kujira.pupmos.network",
    bip44: {
        coinType: 118,
    },
    bech32Config: {
        bech32PrefixAccAddr: "kujira",
        bech32PrefixAccPub: "kujira" + "pub",
        bech32PrefixValAddr: "kujira" + "valoper",
        bech32PrefixValPub: "kujira" + "valoperpub",
        bech32PrefixConsAddr: "kujira" + "valcons",
        bech32PrefixConsPub: "kujira" + "valconspub",
    },
    currencies: [ 
        { 
            coinDenom: "KUJI", 
            coinMinimalDenom: "ukuji", 
            coinDecimals: 6, 
            coinGeckoId: "kujira", 
        }, 
    ],
    feeCurrencies: [
        { 
            coinDenom: "KUJI", 
            coinMinimalDenom: "ukuji", 
            coinDecimals: 6, 
            coinGeckoId: "kujira", 
        },
    ],
    stakeCurrency: { 
            coinDenom: "KUJI", 
            coinMinimalDenom: "ukuji", 
            coinDecimals: 6, 
            coinGeckoId: "kujira", 
    },
    coinType: 118,
    gasPriceStep: {
        low: 0.01,
        average: 0.025,
        high: 0.03,
    },
});
```

## 4) Paste the code in ``Console`` tab.

![](https://www.synergynodes.com/images/kujira-testnet-keplr/Kujira-Testnet-Keplr-03-min.png)

## 5) Press ``Enter``.

![](https://www.synergynodes.com/images/kujira-testnet-keplr/Kujira-Testnet-Keplr-04-min.png)

## 6) Click on ``Approve`` button on Keplr Wallet window.

![](https://www.synergynodes.com/images/kujira-testnet-keplr/Kujira-Testnet-Keplr-05-min.png)

## 7) Close Keplr Wallet and re-open it.

## 8) Click on the networks preset at top of Keplr Wallet, scroll down, and select ``Kujira Testnet``.

![](https://www.synergynodes.com/images/kujira-testnet-keplr/Kujira-Testnet-Keplr-06-min.png)

## 9) The wallet is ready and you can copy the address.

NOTE: After adding Kujira testnet to Keplr wallet, you can import the wallet using the backed up Mnemonic phrase.

![](https://www.synergynodes.com/images/kujira-testnet-keplr/Kujira-Testnet-Keplr-07-min.png)
