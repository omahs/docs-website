# Hourly Reference Rates Methodology

The full text of this methodology can be downloaded as a pdf document using the link below.&#x20;

{% file src="../../.gitbook/assets/reference-rates-methodology.pdf" %}

## Introduction

Coin Metrics produces the Coin Metrics Hourly Reference Rates (the “Reference Rates”), a collection of reference rates quoted in U.S. dollars and other currencies, published once per hour, for a set of cryptocurrencies and fiat currencies. The Reference Rates are designed to serve as a transparent and independent pricing source that promotes the functioning of efficient markets, reduces information asymmetries among market participants, facilitates trading in standardized contracts, and accelerates the adoption of cryptocurrencies as an asset class with the highest standards. The Reference Rates are calculated using a robust and resilient methodology that is resistant to manipulation and applies international best practices for financial benchmarks, including the International Organization of Securities Commissions’ (IOSCO) Principles for Financial Benchmarks. The Coin Metrics Oversight Committee (the “Oversight Committee”) and an independent governance structure protect the integrity of the Reference Rates and ensure the Reference Rates serve as a source of transparent and independent pricing.

## Description

The Reference Rates are published hourly, every day of the year, and represent the reference rate of one unit of the asset quoted in U.S. dollars or other currency. The Reference Rates are calculated at the end of every hour (the “Calculation Time”) and are published within 5 minutes (the “Publication Time”).

## Coverage Universe

The set of assets included in the Hourly Reference Rates coverage universe are included in Appendix A.

## Data and Calculation Methodology

### Data Sources

The input data source for the Reference Rates are markets traded on cryptocurrency exchanges that are approved to serve as pricing sources by the Oversight Committee. The Oversight Committee evaluates markets using a Market Selection Framework that assesses markets along a wide set of criteria to determine if the data source reflects trading activity in a transparent and representative manner. The Oversight Committee evaluates new markets for inclusion as constituent markets and evaluates existing constituent markets using the Market Selection Framework on a quarterly basis or as market conditions warrant. Markets that are approved by the Oversight Committee are added to a list of constituent markets (the “Constituent Markets”). A separate list of Constituent Markets is maintained for each of the Reference Rates in the coverage universe.

A candidate market can be nominated for inclusion and an existing constituent market can be nominated for exclusion by any member of the public or member of the Oversight Committee. Public nominations for inclusion or exclusion of a market can be submitted in writing to `support@coinmetrics.io`. The Oversight Committee may convene to apply the Market Selection Framework to evaluate the inclusion or exclusion of a market between regularly-scheduled quarterly meetings if market conditions or circumstances warrant. Coin Metrics publishes a current list of Constituent Markets for each asset in the Reference Rates coverage universe, updates on inclusions or exclusions of constituent markets, and the rationale for making any change.

### Market Selection Framework

The Market Selection Framework consists of a fully-systematized process for evaluating markets to serve as input pricing sources for the calculation of the Reference Rates. It produces a unique set of candidate markets for each asset in the coverage universe that are then subsequently reviewed by the Oversight Committee. The market selection framework evaluates markets based on the following criteria:

1. _Technology_: An assessment of whether the technology infrastructure of the market’s exchange provides sufficient availability and reliability for input data collection. Evaluates whether the exchange offers a REST API, Websocket feed, or FIX API suitable for data collection. Evaluates the performance of the API in terms of reliability and latency.
2. _Legal and Compliance_: An assessment of selected indicator variables relating to compliance and risk for each exchange. These indicator variables include whether the exchange has publicly-disclosed trading policies, uses market surveillance technology, obtains regulatory licenses, has fiat and crypto insurance, requires customers to verify their identity before opening an account as part of its KYC and AML process, and whether the exchange has functioning fiat and cryptocurrency withdrawals processed within a normal timeframe.&#x20;
3. _Business Model_: An assessment of the market’s exchange with respect to its business model, including its fee structure and asset listing standards.
4. _Data Availability_: An assessment of the available data the market’s exchange offers for the given asset, including the number of markets where the given asset is the base currency, whether the markets are quoted in fiat currencies or other cryptocurrencies, and the type of markets offered.
5. _Price_: An assessment of the quality of the market’s price data, including testing for the occurrence of price outliers and impactful price deviations from other markets, and implementing tests that determine whether the market functions as an active market in the underlying asset and are anchored by observable transactions entered into at arm’s length between buyers and sellers.
6. _Volume_: An assessment of the quality of the market’s volume data, including testing for manipulated volume figures, and implementing tests that determine whether the market functions as an active markets in the underlying asset and are anchored by observable transactions entered into at arm’s length between buyers and sellers. The size of the exchange’s markets are also considered.
7. _Order Book_: An assessment of the quality of the market’s order book data, including tests for manipulated orders, and implementing tests that determine whether the market functions as an active market in the underlying asset and are anchored by observable transactions entered into at arm’s length between buyers and sellers. The liquidity of the market is also considered.

The full Market Selection Framework can be found [here](https://docs.coinmetrics.io/methodologies/reference-rates/market-selection-framework).

### Data Inputs

The data inputs for the calculation of the Reference Rates are observable transactions in an active market where the given asset is traded. The pool of candidate markets that are evaluated by the Market Selection Framework are determined by a hierarchy of data inputs that varies depending on the given asset.

#### Bitcoin (BTC) and Ethereum (ETH)

The pool of candidate markets that are evaluated for the calculation of the Reference Rates for Bitcoin (BTC) and Ethereum (ETH) are determined using the following data hierarchy:

1. The primary data input is observable transactions in an active market where the given cryptocurrency is the base currency and the quote currency is U.S. dollars.
2. Markets where the given cryptocurrency is the base currency and the quote currency is not U.S. dollars are not considered, including markets quoted in other fiat currencies or markets quoted in stablecoins.

#### Other Cryptocurrencies Excluding Stablecoins

The pool of candidate markets that are evaluated for the calculation of the Reference Rates for other cryptocurrencies, excluding Bitcoin (BTC), Ethereum (ETH), and stablecoins are determined using the following data hierarchy:

1. The primary data input is observable transactions in an active market where the given cryptocurrency is the base currency and the quote currency is U.S. dollars.
2. If the above data inputs do not exist or the Oversight Committee makes a determination that the above data inputs are insufficient to calculate the reference rate, the universe of data inputs will expand to include observable transactions in an active market where the given cryptocurrency is the base currency and quote currency is Bitcoin (BTC).
3. If the above data inputs do not exist or the Oversight Committee makes a determination that the above data inputs are insufficient to calculate the reference rate, the universe of data inputs will expand to include observable transactions in an active market where the given cryptocurrency is the base currency and quote currency is Ethereum (ETH).
4. If the above data inputs do not exist or the Oversight Committee makes a determination that the above data inputs are insufficient to calculate the reference rate, the universe of data inputs will expand to include observable transactions in an active market where the given cryptocurrency is the base currency and quote currency is USD Coin (USDC).
5. If the above data inputs do not exist or the Oversight Committee makes a determination that the above data inputs are insufficient to calculate the reference rate, the universe of data inputs will expand to include observable transactions in an active market where the given cryptocurrency is the base currency and quote currency is Tether (USDT).

#### Stablecoins

The pool of candidate markets that are evaluated for the calculation of the Reference Rates for stablecoins are determined using the following data hierarchy:

1. The primary data input is observable transactions in an active market where the given stablecoin is the base currency and the quote currency is U.S. dollars.
2. If the above data inputs do not exist or the Oversight Committee makes a determination that the above data inputs are insufficient to calculate the reference rate, the universe of data inputs will expand to include observable transactions in an active market where Bitcoin (BTC) is the base currency and quote currency is the given stablecoin.
3. If the above data inputs do not exist or the Oversight Committee makes a determination that the above data inputs are insufficient to calculate the reference rate, the universe of data inputs will expand to include observable transactions in an active market where Ethereum (ETH) is the base currency and quote currency is the given stablecoin.
4. If the above data inputs do not exist or the Oversight Committee makes a determination that the above data inputs are insufficient to calculate the reference rate, the universe of data inputs will expand to include observable transactions in an active market where the given stablecoin is the base currency and quote currency is USD Coin (USDC).
5. If the above data inputs do not exist or the Oversight Committee makes a determination that the above data inputs are insufficient to calculate the reference rate, the universe of data inputs will expand to include observable transactions in an active market where the given stablecoin is the base currency and quote currency is Tether (USDT).

The data hierarchy for stablecoins differs from other cryptocurrencies because market convention sets stablecoins as the quote currency for the majority of active markets. The following assets in the coverage universe are considered to be stablecoins:

| Name           | Ticker |
| -------------- | ------ |
| Tether         | usdt   |
| TrueUSD        | tusd   |
| USD Coin       | usdc   |
| Paxos Standard | pax    |
| Gemini Dollar  | gusd   |
| HUSD           | husd   |
| Binance USD    | busd   |
| Dai            | dai    |
| USDK           | usdk   |
| Binance IDR    | bidr   |
| sUSD           | susd   |
| Neutrino USD   | usdn   |
| TerraUSD       | ust    |
| mStable USD    | musd   |
| USD Paxos      | usdp   |

#### Fiat Currencies

The pool of candidate markets that are evaluated for the calculation of the Reference Rates for fiat currencies are determined using the following data hierarchy:

1. The primary data input is observable transactions in an active market where the given fiat currency is the base currency and the quote currency is U.S. dollars.
2. If the above data inputs do not exist or the Oversight Committee makes a determination that the above data inputs are insufficient to calculate the reference rate, the universe of data inputs will expand to include observable transactions in an active market where Bitcoin (BTC) is the base currency and quote currency is the given fiat currency.
3. If the above data inputs do not exist or the Oversight Committee makes a determination that the above data inputs are insufficient to calculate the reference rate, the universe of data inputs will expand to include observable transactions in an active market where Ethereum (ETH) is the base currency and quote currency is the given fiat currency.

The data hierarchy for fiat currencies differs from other cryptocurrencies because market convention sets fiat currencies as the quote currency for the majority of active markets. The following assets in the coverage universe are considered to be fiat currencies:

| Name              | Ticker |
| ----------------- | ------ |
| Euro              | eur    |
| British Pound     | gbp    |
| Japanese Yen      | jpy    |
| Canadian Dollar   | cad    |
| Korean won        | krw    |
| Russian Ruble     | rub    |
| Ukrainian Hryvnia | uah    |
| Turkish Lira      | try    |
| Australian Dollar | aud    |
| Brazilian Real    | brl    |
| Swiss Franc       | chf    |
| Hong Kong Dollar  | hkd    |
| Nigerian Naira    | ngn    |
| Singapore Dollar  | sgd    |

### Calculation Algorithm

The calculation algorithm of the Reference Rates is described below.

1. All observable transactions from Constituent Markets are combined and partitioned into time intervals, with each time interval spanning a period of one minute. The first one-minute time interval begins 60 minutes before the Calculation Time and the last one-minute time interval begins at the Calculation and ends one minute after the Calculation Time. In total, the calculation period spans a period of 61 minutes (the “Observation Window”). A total of 61 one-minute time intervals are created.
2. The price of each observable transaction for one unit of the given asset is converted to U.S. dollars if necessary using the Reference Rates calculated for Bitcoin (BTC) or Ethereum (ETH).
3. The volume-weighted median price (VWMP) of each time interval is calculated. The volume-weighted median rate is calculated by ordering the transactions from lowest to highest price, taking the cumulative sum of volumes of these transactions, and identifying the price associated with the trades at the 50th percentile of volume measured in native units.
4. The time-weighted average price (TWAP) of the 61 time intervals is calculated using a custom weight function. The weight function assigns a weight of 0 percent to the first time interval, subsequent time intervals are assigned a weight that increases linearly, and the last two time intervals are assigned a weight of 5 percent such that the sum of all weights equals 100 percent. The weight function assigns more weight to time slices that are closer to the Calculation Time. The resulting figure is the published reference rate.

A chart of the weights is included below and the exact weights for each time interval are listed in Appendix B:

![](../../.gitbook/assets/image.png)

### Data Contingency Rules

The following contingency rules are followed to address situations where data is delayed, missing, or unavailable due to periods of illiquidity, extraordinary market circumstances, or outside factors beyond the control of Coin Metrics.

1. If observable transactions from a constituent market are unable to be collected due to technical problems specific to the constituent market’s exchange during the calculation of a reference rate, the observable transactions from the constituent market are not included in the calculation of the specific instance of the given reference rate.
2. If no observable transactions from constituent markets occur during the first one-minute time interval, the next one-minute time interval’s volume-weighted median price is used as the volume-weighted median price. This contingency rule is applied recursively if necessary.
3. If no observable transactions from constituent markets occur during any one-minute time intervals, excluding the first and last one-minute time intervals in the Calculation Window, the next one-minute time interval’s volume-weighted median price is used as the volume-weighted median price. This contingency rule is applied recursively if necessary.
4. If no observable transactions from constituent markets occur during the last one-minute time interval, the previous time interval’s volume-weighted median price is used as the volume-weighted median price. This contingency rule is applied recursively if necessary.
5. If no observable transactions from constituent markets exist during the Calculation Period for a reference rate, the reference rate will be determined to equal the previous hourly reference rate in which there were trades during that hour’s Observation Window.

### Data Exclusion Rules

All observable transactions from constituent markets are evaluated using a systematic data quality control process. If potential errors or anomalies in the data are detected, the exercise of expert judgment will be applied to determine if the potentially erroneous data is included in the calculation of the reference rate. The exercise of expert judgment in this circumstance is used to determine if the potentially erroneous data reflects observable transactions that are entered into at arm’s length between buyers and sellers and constitute an active market in the underlying asset, whether the observable transactions in question are formed by the competitive forces of supply and demand, and whether the observable transactions in question are a credible indicator of executable prices in the underlying asset. An investigation into the causes of the potential error, including whether any price deviations are specific to the exchange itself, is conducted. Any exercise of expert judgment is subject to dual approval by staff members, and is logged and reported to the Oversight Committee which periodically reviews the application of expert judgment to ensure consistency.

## Recalculations

If errors are discovered in the calculation process subsequent to the publication of the reference rate, a recalculated reference rate may be published. Such errors can include the following events:

1. A constituent market begins trading at a spread against other constituent markets due to a temporary halting of withdrawals or deposits or an increase in solvency risk for a specific exchange
2. A constituent market is temporarily halted due to unplanned exchange maintenance
3. Data from constituent markets is interrupted due to network delays or instability
4. Data from constituent markets is interrupted due to an unplanned change in an exchange’s API
5. Suspected trade manipulation is observed on a constituent market
6. A ticker change or token swap for a constituent market is missed or misapplied
7. Calculation methodology is incorrectly applied

Recalculations to the reference rates are assessed on a case-by-case basis in consultation with the Oversight Committee. Decisions regarding recalculations take into consideration all the available data and the potential negative impact or disruption involved in a recalculation. All recalculations are announced simultaneously to all clients.

## Administration

Coin Metrics serves as the administrator for the Reference Rates and has primary responsibility for all aspects of the Reference Rates determination process, including the development, definition, determination, dissemination, operation, and governance of the Reference Rates. All aspects of the production of the Reference Rates are carried out by Coin Metrics, and Coin Metrics does not rely on any third parties for the determination of the Reference Rates.

Coin Metrics ensures that transparency regarding significant decisions and associated rationale are published and made available to external stakeholders. Data contingency and data exclusion rules are in place to handle certain extraordinary circumstances and external factors beyond the control of Coin Metrics. The Oversight Committee reviews and provides challenge on the Reference Rates production process.

## Internal Oversight

The Oversight Committee provides independent oversight over the production of the Reference Rates. The Oversight Committee’s responsibilities include regular reviews of the Reference Rate production process, the Reference Rate definition and calculation methodology, the selection of data sources and data inputs, any uses of expert judgment or non-standard procedures, conflicts of interest, material changes to or termination of the Reference Rates, reviewing the results of external and internal audits, and any complaints or questions regarding the Reference Rates from external stakeholders. Additional information regarding the responsibilities and membership of the Oversight Committee can be found in the Coin Metrics Oversight Committee Charter document.

## Conflicts of Interest

Coin Metrics enforces policies and procedures relating to conflicts of interest in connection with the production of the Reference Rates. The conflicts of interest policy addresses the identification, disclosure, management, and mitigation of conflicts of interest. These policies and procedures are periodically reviewed by the Oversight Committee. Coin Metrics is committed to disclosing any material conflicts of interest to external stakeholders and to regulatory authorities.

## Material Changes or Termination

Coin Metrics may initiate material changes to or terminate a reference rate due to certain extraordinary market circumstances or external factors. These circumstances or external factors include, but are not limited to:

1. The reference rate no longer serves, and could not be modified to serve, as a transparent and independent pricing source for the underlying asset
2. The market liquidity in the underlying asset declines to an extent that the input data sources no longer function as active markets
3. The underlying asset experiences a contentious hard fork in which both forks survive

In such circumstances, Coin Metrics will review the Reference Rates to ensure the Reference Rates are properly reflecting their underlying assets, and if necessary, make changes to the methodology or definition of the Reference Rates to properly account for changing market structure, circumstances, and industry conventions in the underlying asset. Any such change or termination will be reviewed and approved by the Oversight Committee. Any approved change or termination will be publicly disclosed to external stakeholders with a detailed explanation of the rationale. In a manner appropriate to the circumstances, Coin Metrics will develop a plan to notify, solicit comments from, and consult with external stakeholders before implementing any material change or termination. Any change or termination will include a timeline explaining the timing of changes or termination and include steps to mitigate any negative effects on external stakeholders.

## Internal Controls

Coin Metrics has implemented internal controls to protect the integrity of the Reference Rates. These controls cover the selection of input data sources, the collection of data from input data sources, and maintaining the integrity of collected data. Staff involved with the production of the Reference Rates have been trained in the proper usage of the data and maintain proper segregation of responsibilities. Any exercise of expert judgment or non-standard procedures is subject to dual approval by staff members, and is logged and reported to the Oversight Committee which periodically reviews any incidents. In addition, Coin Metrics maintains a whistleblowing mechanism to facilitate the reporting of any potential misconduct.

## Complaints

Complaints about the calculation methodology of the Reference Rates or the value of a published reference rate should be submitted in writing to `support@coinmetrics.io`. Coin Metrics will investigate any complaints and respond to the complainant in a fair and timely manner. Any investigation of the complaint will adhere to the following procedures:

1. The personnel receiving and investigating the complaint will be independent of any personnel who may have been involved in the subject of the complaint.
2. All records and documents submitted by the complainant and related to the investigation into the complaint will be retained for a period of at least five years and submitted to the Oversight Committee for review.
3. Any complaint that results in a change in the determination of the Reference Rates, its calculation methodology, or its policies will be publicly disclosed and will explain the action taken.

## Record Retention

Coin Metrics retains records, for at least five years, on the following items:

1. All market data that is collected and used in the calculation of the Reference Rates
2. Any use of expert judgment in the calculation of the Reference Rates
3. Any use of non-standard procedures in the calculation of the Reference Rates
4. The identities of staff responsible for the calculation of the Reference Rates
5. Any responses, questions, or complaints received in connection with the calculation of the Reference Rates

## Compliance

Coin Metrics maintains records and has processes in place to comply with requests for information from regulatory authorities. Coin Metrics commits to full cooperation with any regulatory authority in carrying out their regulatory or supervisory duties.

## Change Log

1. **Version 2.13 on September 21, 2022**: The coverage universe is expanded to include the following assets: `loka`, `mc`, `polis`, `sgb`, `steth`, `frax`, `rai`, `lusd` , `dfi`, `gbpt`, `ooki`, `fis`, `nest`, `drep`, `math`, `aleph`, `media`, `luna2`, `t`, `ethw`, `bttc`, `vra`, `swftc`, `raca`, `pyr`, `mbox`, `sweat`, `fitfi`, `qrdo`, `wemix`, `zbc`, `psg`, `voxel`, `chess`, `prq`, `gari`, `nym`, `arv`, `cudos`, `efi`, `for`, `juv`, `cvp`, `mbl`, `auto`, `eden`, `xcn`, `kai`, `velo`, `akt`, `berry`, `klv`, `kok`, `senso`, `floki`, `sdn`, `alpine`, `step`, `eurt`, `bfc`, `toke`, `shping`, `oxy`, `ssx`, `lit`, `conv`. The publication of reference rates is termintaed for the following assets: `ramp`, `grs`, `ppt`, `nav`, `itc`, `qc`, `meta`, `cope`, `zb`. Minor changes to internal audit section.
2. **Version 2.12 on July 1, 2022**: The coverage universe is expanded to include the following assets: `fei`, `op`, `usdd`, `xch`, `gmt`, `bico`, `ctk`, `flm`, `sfp`, `starl`, `glmr`, `tulip`, `astro`, `sfi`, `gst`, `mob`, `bit`, `vgx`, `auction`, `pundix`, `stg`, `ata`, `bel`, `dar`, `gal`, `astr`, `cqt`, `cspr`, `metis`, `boba`, `twt`, `aca`, `dao`, `xprt`, `cube`. The publication of reference rates is terminated for the following assets: `gxs`, `dgtx`, `wluna`, `dgd`, `foam`, `csp`, `cnn`, `bft`.
3. **Version 2.11 on February 15, 2022**: The coverage universe is expanded to include the following assets: `xec`, `kda`, `mina`, `xdc`, `elon`, `flux`, `movr`, `ceek`, `win_wink`, `dvi`, `dusk`, `asd`, `gala`, `spell`, `ens`, `tru`, `alcx`, `clv`, `imx`, `agld`, `jasmy`, `farm`, `alice`, `chr`, `dydx`, `tlm`, `mdt`, `gtc`, `sun`, `c98`, `people`, `lina`, `rndr`, `ach`, `super`, `mask`, `quick`, `arpa`, `qi`, `idex`, `rad`, `bond`, `mir`, `joe`, `gods`, `front`, `pla`, `orn`, `ramp`, `rgt`, `fida`, `forth`, `tribe`, `wluna`, `coval`, `rbn`, `lcx`, `asm`, `ddx`, `suku`, `krl`, `rari`, `mco2`, `gyen`, `btrst`, `api3`, `rly`, `wcfg`, `musd`, `ilv`, `atlas`, `usdp`, `joe`, `ldo`, `cvx`, `fxs`, `kp3r`, `alpaca`, `bnx`, `boson`, `dora`, `ghst`, `nft`, `ohm`, `om`, `pond`, `rare`, `revv`, `stpt`, `torn`, `tvk`, `wncg`, `xym`, `ygg`. The publication of reference rates is terminated for the following assets: `hedg`, `eurs`, `bzrx`, `poa`, `wpr`, `dmg`, `cdt`, `phx`, `appc`, `btt`, `idrt`, `rdn`, `via`, `evx`. The section “Data Inputs”, subsections “Other Cryptocurrencies Excluding Stablecoins” and “Stablecoins”, was modified to consider markets quoted in USD Coin or Tether to serve as constituent markets. The constituent markets for all assets in the coverage universe are updated. The constituent markets for all assets in the coverage universe are updated.
4. **Version 2.10 on September 28, 2021**: The coverage universe is expanded to include the following assets: `amp`, `axs`, `shib`, `audio`, `bake`, `med`, `dag`, `slp`, `xdb`. The publication of reference rates is terminated for the following assets: `agi` ,`btmx`, `dgx`, `ethos`, `mco`, `sngls`, `cpay`, `eng`, `lun`, `pnt`. The constituent markets for all assets in the coverage universe are updated.
5. **Version 2.9 on May 27, 2021**: The coverage universe is expanded to include the following assets: `icp`, `cope`, `maps`, `btcst`, `ctsi`, `erg`, `woo`, `prom`, `strax`, `usdn`, `cfx`, `mdx`, `nkn`, `sand`, `fx`, `pha`. The publication of reference rates is terminated for the following assets: `tnt`, `npxs`, `zar`. The constituent markets for all assets in the coverage universe are updated.
6. **Version 2.8 on April 25, 2021**: The methodology was modified to add fiat currencies to the coverage universe. The coverage universe is expanded to include the following assets: `eur`, `krw`, `gbp`, `jpy`, `aud`, `try`, `brl`, `rub`, `sgd`, `bidr`, `ngn`, `cad`, `chf`, `zar`, `idrt`, `hkd`, `uah`, `qc`, `klay`, `cake`, `btmx`, `flow`, `zks`, `stmx`, `skl`, `reef`, `dodo`, `coti`, `bora`, `cream`, `ray`, `tryb`, `rook`. The publication of reference rates is terminated for the following assets: `xzc`, `bcpt`, `yamv2`, `xns`, `tmtg`, `kp3r`.
7. **Version 2.7 on February 23, 2021**: The coverage universe is expanded to include the following assets: `1inch`, `alpha`, `octo`, `perp`, `scrt`, `grt`, `keep`, `xvs`, `nu`, `tel`, `badger`.
8. **Version 2.6 on January 26, 2021**: The coverage universe is expanded to include the following assets: `susd`, `pols`, `ust`, `lto`, `swap`, `nim,` `lbc`, `mta`, `kp3r`, `glm`, `near`, `noia`, `rose`, `inj`. The publication of reference rates is terminated for the following assets: `gnt`, `fxc`, `bht`, `cmct`, `strat`, `loki`. The constituent markets for all assets in the coverage universe are updated.
9. **Version 2.5 on November 5, 2020**: The coverage universe is expanded to include the following assets: `akro`, `ampl`, `ar`, `bal`, `bzrx`, `celo`, `comp`, `crv`, `csp`, `dmg`, `dot`, `foam`, `kin`, `oxt`, `rune`, `sol`, `srm`, `vtho`, `wbtc`, `wnxm`, `xhv`, `xyo`, `yamv2`, `yfi`, `yfii`, `uma`, `ewt`, `rev`, `rsr`, `avax`, `tmtg`, `jst`, `hnt`, `trac`, `vlx`, `mxc`, `fet`, `aoa`, `iris`, `pnk`, `mln`, `shr`, `uqc`, `one_harmony`, `trb`, `ogn`, `ava`, `loki`, `hxro`, `wxt`, `cpay`, `fil`, `uni`, `swrv`, `sushi`, `aave`, `egld`, `hns`, `dia`, `boa`, `uos`, `ctc`, `renbtc`. The publication of reference rates is terminated for the following assets: `arn`, `pma`, `erd`, `man`, `iq`, `lend`. The Market Selection Framework was amended such that extremely low volume markets are less likely to be selected as a constituent market if higher volume markets of similar quality are available. The constituent markets for all assets in the coverage universe are updated.
10. **Version 2.4 on July 29, 2020**: The coverage universe is expanded to include the following assets: `wrx`, `band`, `ksm`, `usdk`, `snx`, `stx`, `fxc`, `kcs`, `hive`, `nrg`, `cel`, `ubt`, `chsb`, `crpt`, `bht`, `cvt`, `data`, `eurs`, `xns`, `gt`, `dgtx`, `kava`, `tt`, `sxp`, `mx`, `ocean`, `erd`, `lpt`. The publication of reference rates is terminated for the following assets: `storm`, `gto`. A revision policy was amended. The constituent markets for all assets in the coverage universe are updated.
11. **Version 2.3 on February 27, 2020**: The coverage universe is expanded to include the following assets: `xaut`, `paxg`, `husd`, `dgx`, `busd`, `ftt`, `hedg`, `okb`, `zb`, `hbar`, `ckb`, `mof`, `vsys`, `cennz`, `luna`, `chz`, `seele`, `dx`, `matic`, `abbc`, `rif`, `tomo`, `hpt`, and `ant`.
12. **Version 2.2 on February 6, 2020**: The constituent markets for all assets in the coverage universe are updated. The coverage universe is adjusted to remove the following assets: `box`, `cosm`, `fsn`, `medx`, `pst`, and `ttc_protocol`. The coverage universe was expanded to include Dai and the previous asset with this name was renamed to Sai to appropriately reflect MakerDAO’s transition from Single-Collateral Dai (Sai) to Multi-Collateral Dai (Dai).
13. **Version 2.1 on December 9, 2019**: The coverage universe is expanded to include the following assets: `algo` and `beam`.
14. **Version 2.0 on July 8, 2019**: Increased publication times from once daily at midnight UTC to once hourly. Changed human oversight from once daily at midnight UTC to once daily at 16:00 New York time.
15. **Version 1.2 on June 13, 2019**: The coverage universe is expanded to include the following assets: `gno`, `hot_holo`, `maid`, `nuls`, `qkc`, `rdd`, `rvn`, `zen`, and `mona`.
16. **Version 1.1 on May 30, 2019**: Updated data contingency rules. If no observable transactions from constituent markets occur during a one-minute time interval, the next one-minute time interval’s volume-weighted median price is used instead of the previous. This contingency rule is applied recursively.
17. **Version 1.0 on May 13, 2019**: Initial publication of Reference Rates Methodology.

## Appendix A

The following table lists the current coverage universe:

| Name                                 | Ticker                  |
| ------------------------------------ | ----------------------- |
| Bitcoin                              | btc                     |
| Bitcoin Cash                         | bch                     |
| Litecoin                             | ltc                     |
| Euro                                 | eur                     |
| XRP                                  | xrp                     |
| Ethereum                             | eth                     |
| Ethereum Classic                     | etc                     |
| British Pound                        | gbp                     |
| Zcash                                | zec                     |
| Monero                               | xmr                     |
| Dash                                 | dash                    |
| Japanese Yen                         | jpy                     |
| IOTA                                 | miota                   |
| EOS                                  | eos                     |
| OMG Network                          | omg                     |
| Neo                                  | neo                     |
| Metaverse ETP                        | etp                     |
| Qtum                                 | qtum                    |
| Aventus                              | avt                     |
| Bitcoin Gold                         | btg                     |
| Streamr                              | data                    |
| QASH                                 | qash                    |
| Status                               | snt                     |
| Basic Attention Token                | bat                     |
| Decentraland                         | mana                    |
| FUNToken                             | fun                     |
| 0x                                   | zrx                     |
| Time New Bank                        | tnb                     |
| TRON                                 | trx                     |
| iExec RLC                            | rlc                     |
| Augur                                | rep                     |
| aelf                                 | elf                     |
| IOST                                 | iost                    |
| Aion                                 | aion                    |
| Request                              | req                     |
| Loopring                             | lrc                     |
| WAX                                  | waxp                    |
| Aragon                               | ant                     |
| Mithril                              | mith                    |
| Storj                                | storj                   |
| Stellar                              | xlm                     |
| Verge                                | xvg                     |
| Lympo                                | lym                     |
| Maker                                | mkr                     |
| VeChain                              | vet                     |
| Kyber Network Crystal                | knc                     |
| Utrust                               | utk                     |
| Ripio Credit Network                 | rcn\_ripiocreditnetwork |
| Polymath                             | poly                    |
| Nitro Network                        | ncash                   |
| Cortex                               | ctxc                    |
| Project Pai                          | pai                     |
| DATA                                 | dta                     |
| Zilliqa                              | zil                     |
| Bancor                               | bnt                     |
| MonaCoin                             | mona                    |
| NEM                                  | xem                     |
| BNB                                  | bnb                     |
| Gas                                  | gas                     |
| Tether                               | usdt                    |
| OAX                                  | oax                     |
| district0x                           | dnt                     |
| Waltonchain                          | wtc                     |
| Chainlink                            | link                    |
| Moeda Loyalty Points                 | mda                     |
| Metal                                | mtl\_metal              |
| AirSwap                              | ast                     |
| Viberate                             | vib                     |
| Powerledger                          | powr                    |
| Ark                                  | ark                     |
| Enjin Coin                           | enj                     |
| Komodo                               | kmd                     |
| NULS                                 | nuls                    |
| Ambrosus                             | amb                     |
| Quantstamp                           | qsp                     |
| BitShares                            | bts                     |
| Lisk                                 | lsk                     |
| Bitcoin Diamond                      | bcd                     |
| Ambire AdEx                          | adx                     |
| Cardano                              | ada                     |
| CyberMiles                           | cmt                     |
| Waves                                | waves                   |
| ICON                                 | icx                     |
| PIVX                                 | pivx                    |
| OST                                  | ost                     |
| ChatCoin                             | chat                    |
| Civic                                | cvc                     |
| Steem                                | steem                   |
| Nano (New)                           | nano                    |
| Bluzelle                             | blz                     |
| Aeternity                            | ae                      |
| Ontology                             | ont                     |
| Wanchain                             | wan                     |
| Syscoin                              | sys                     |
| Ardor                                | ardr                    |
| Holo                                 | hot\_holo               |
| Loom Network                         | loom                    |
| Bytecoin                             | bcn                     |
| TrueUSD                              | tusd                    |
| Horizen                              | zen                     |
| Theta Network                        | theta                   |
| IoTeX                                | iotx                    |
| QuarkChain                           | qkc                     |
| SelfKey                              | key                     |
| Hifi Finance                         | mft                     |
| Siacoin                              | sc                      |
| Nebulas                              | nas                     |
| Dent                                 | dent                    |
| Dock                                 | dock                    |
| Gnosis                               | gno                     |
| Canadian Dollar                      | cad                     |
| Enzyme                               | mln                     |
| Dogecoin                             | doge                    |
| Bytom                                | btm                     |
| BitKan                               | kan                     |
| Arcblock                             | abt                     |
| Auto                                 | auto                    |
| CyberVein                            | cvt                     |
| Decred                               | dcr                     |
| DigiByte                             | dgb                     |
| Cred                                 | lba                     |
| Measurable Data Token                | mdt                     |
| Molecular Future                     | mof                     |
| TenX                                 | pay                     |
| Revain                               | rev                     |
| Ren                                  | ren                     |
| SwftCoin                             | swftc                   |
| Nxt                                  | nxt                     |
| Odyssey                              | ocn                     |
| Huobi Token                          | ht                      |
| Elastos                              | ela                     |
| WaykiChain                           | wicc                    |
| SIRIN LABS Token                     | srn                     |
| DeepBrain Chain                      | dbc                     |
| Propy                                | pro                     |
| Bibox Token                          | bix                     |
| HyperCash                            | hc\_hypercash           |
| MaidSafeCoin                         | maid                    |
| Amp                                  | amp                     |
| Pluton                               | plu                     |
| Tezos                                | xtz                     |
| Stacks                               | stx                     |
| Ignis                                | ignis                   |
| PolySwarm                            | nct                     |
| Kin                                  | kin                     |
| SwissBorg                            | chsb                    |
| CENNZnet                             | cennz                   |
| OriginTrail                          | trac                    |
| Nexo                                 | nexo                    |
| Telcoin                              | tel                     |
| Berry                                | berry                   |
| Crypterium                           | crpt                    |
| IHT Real Estate Protocol             | iht                     |
| VeThor Token                         | vtho                    |
| DxChain Token                        | dx                      |
| CEEK VR                              | ceek                    |
| Oxygen                               | oxy                     |
| UNUS SED LEO                         | leo                     |
| Factom                               | fct                     |
| Vertcoin                             | vtc                     |
| Game.com                             | gtc\_gamecom            |
| MediBloc                             | med                     |
| Creditcoin                           | ctc                     |
| NKN                                  | nkn                     |
| Uquid Coin                           | uqc                     |
| Korean won                           | krw                     |
| Ravencoin                            | rvn                     |
| LBRY Credits                         | lbc                     |
| ReddCoin                             | rdd                     |
| Numeraire                            | nmr                     |
| Russian Ruble                        | rub                     |
| Ukrainian Hryvnia                    | uah                     |
| Turkish Lira                         | try                     |
| Aurora                               | aoa                     |
| Australian Dollar                    | aud                     |
| Brazilian Real                       | brl                     |
| Swiss Franc                          | chf                     |
| Ethernity                            | ern                     |
| Hong Kong Dollar                     | hkd                     |
| Singapore Dollar                     | sgd                     |
| OpenDAO                              | sos                     |
| Dragonchain                          | drgn                    |
| Kleros                               | pnk                     |
| USD Coin                             | usdc                    |
| KuCoin Token                         | kcs                     |
| Paxos Standard                       | pax                     |
| Gemini Dollar                        | gusd                    |
| Constellation                        | dag                     |
| Nimiq                                | nim                     |
| GoChain                              | go                      |
| Electroneum                          | etn                     |
| Bitcoin SV                           | bsv                     |
| MXC                                  | mxc                     |
| TomoChain                            | tomo                    |
| Livepeer                             | lpt                     |
| RSK Infrastructure Framework         | rif                     |
| v.systems                            | vsys                    |
| Grin                                 | grin                    |
| Seele                                | seele                   |
| HUSD                                 | husd                    |
| Lambda                               | lamb                    |
| Huobi Pool Token                     | hpt                     |
| Dora Factory                         | dora                    |
| Beam                                 | beam                    |
| Unibright                            | ubt                     |
| FTX Token                            | ftt                     |
| Kryll                                | krl                     |
| Fetch.ai                             | fet                     |
| Ontology Gas                         | ong\_ontologygas        |
| Ankr                                 | ankr                    |
| Haven Protocol                       | xhv                     |
| Quant                                | qnt                     |
| SOLVE                                | solve                   |
| Aergo                                | aergo                   |
| Circuits of Value                    | coval                   |
| Cronos                               | cro                     |
| Hxro                                 | hxro                    |
| Cosmos                               | atom                    |
| Orbs                                 | orbs                    |
| Theta Fuel                           | tfuel                   |
| BORA                                 | bora                    |
| Function X                           | fx                      |
| IRISnet                              | iris                    |
| Celer Network                        | celr                    |
| ABBC Coin                            | abbc                    |
| Verasity                             | vra                     |
| Wrapped Bitcoin                      | wbtc                    |
| Polygon                              | matic                   |
| Litentry                             | lit                     |
| Fantom                               | ftm                     |
| Algorand                             | algo                    |
| Dusk Network                         | dusk                    |
| XYO                                  | xyo                     |
| Ocean Protocol                       | ocean                   |
| Celsius                              | cel                     |
| Synthetix                            | snx                     |
| ThunderCore                          | tt                      |
| MovieBloc                            | mbl                     |
| Reserve Rights                       | rsr                     |
| STP                                  | stpt                    |
| Harmony                              | one\_harmony            |
| ARPA Chain                           | arpa                    |
| WINkLink                             | win\_wink               |
| Binance USD                          | busd                    |
| Dai                                  | dai                     |
| Tether Gold                          | xaut                    |
| PAX Gold                             | paxg                    |
| OKB                                  | okb                     |
| Hedera                               | hbar                    |
| Nervos Network                       | ckb                     |
| SXP                                  | sxp                     |
| Terra Classic                        | luna                    |
| Chiliz                               | chz                     |
| Orchid                               | oxt                     |
| LCX                                  | lcx                     |
| USDK                                 | usdk                    |
| WazirX                               | wrx                     |
| Band Protocol                        | band                    |
| Kusama                               | ksm                     |
| Hive                                 | hive                    |
| Energi                               | nrg                     |
| GateToken                            | gt                      |
| Kava                                 | kava                    |
| MX TOKEN                             | mx                      |
| Arweave                              | ar                      |
| Compound                             | comp                    |
| NuCypher                             | nu                      |
| Keep Network                         | keep                    |
| Origin Protocol                      | ogn                     |
| Render Token                         | rndr                    |
| DREP                                 | drep                    |
| LTO Network                          | lto                     |
| COTI                                 | coti                    |
| Solana                               | sol                     |
| Cartesi                              | ctsi                    |
| Chromia                              | chr                     |
| StormX                               | stmx                    |
| BIDR                                 | bidr                    |
| Polkadot                             | dot                     |
| Celo                                 | celo                    |
| Filecoin                             | fil                     |
| sUSD                                 | susd                    |
| Travala.com                          | ava                     |
| Wirex Token                          | wxt                     |
| Syntropy                             | noia                    |
| Akropolis                            | akro                    |
| Ampleforth                           | ampl                    |
| SENSO                                | senso                   |
| DigitalBits                          | xdb                     |
| Neutrino USD                         | usdn                    |
| KardiaChain                          | kai                     |
| Energy Web Token                     | ewt                     |
| yearn.finance                        | yfi                     |
| UMA                                  | uma                     |
| renBTC                               | renbtc                  |
| Avalanche                            | avax                    |
| BOSAGORA                             | boa                     |
| JUST                                 | jst                     |
| Bifrost                              | bfc                     |
| DIA                                  | dia                     |
| ForTube                              | for                     |
| Green Satoshi Token                  | gst                     |
| Helium                               | hnt                     |
| IDEX                                 | idex                    |
| Kadena                               | kda                     |
| Klaytn                               | klay                    |
| mStable Governance Token: Meta (MTA) | mta                     |
| NEST Protocol                        | nest                    |
| MANTRA                               | om                      |
| Orion Protocol                       | orn                     |
| Prom                                 | prom                    |
| PARSIQ                               | prq                     |
| THORChain                            | rune                    |
| ShareToken                           | shr                     |
| Serum                                | srm                     |
| SUKU                                 | suku                    |
| Tellor                               | trb                     |
| BiLira                               | tryb                    |
| Curve DAO Token                      | crv                     |
| Velas                                | vlx                     |
| Wrapped NXM                          | wnxm                    |
| DFI.Money                            | yfii                    |
| Balancer                             | bal                     |
| SushiSwap                            | sushi                   |
| Swerve                               | swrv                    |
| Cream Finance                        | cream                   |
| Sun Token                            | sun                     |
| Elrond                               | egld                    |
| Uniswap                              | uni                     |
| Alchemy Pay                          | ach                     |
| Aleph.im                             | aleph                   |
| Bella Protocol                       | bel                     |
| Frontier                             | front                   |
| Klever                               | klv                     |
| TrustSwap                            | swap                    |
| TerraUSD                             | ust                     |
| Handshake                            | hns                     |
| Ultra                                | uos                     |
| BakeryToken                          | bake                    |
| Aavegotchi                           | ghst                    |
| Rarible                              | rari                    |
| Velo                                 | velo                    |
| Aave                                 | aave                    |
| PancakeSwap                          | cake                    |
| DODO                                 | dodo                    |
| Harvest Finance                      | farm                    |
| Polkastarter                         | pols                    |
| Secret                               | scrt                    |
| Venus                                | xvs                     |
| Ergo                                 | erg                     |
| MATH                                 | math                    |
| NEAR Protocol                        | near                    |
| DeFiChain                            | dfi                     |
| Audius                               | audio                   |
| Axie Infinity                        | axs                     |
| Conflux                              | cfx                     |
| Shentu                               | ctk                     |
| Injective                            | inj                     |
| Keep3rV1                             | kp3r                    |
| mStable USD                          | musd                    |
| Smooth Love Potion                   | slp                     |
| StaFi                                | fis                     |
| Flamingo                             | flm                     |
| Oasis Network                        | rose                    |
| TrueFi                               | tru                     |
| Unifi Protocol DAO                   | unfi                    |
| Golem                                | glm                     |
| API3                                 | api3                    |
| Badger DAO                           | badger                  |
| MobileCoin                           | mob                     |
| Synapse                              | syn                     |
| Virtua                               | tvk                     |
| The Graph                            | grt                     |
| 1inch                                | 1inch                   |
| Alpha Venture DAO                    | alpha                   |
| OctoFi                               | octo                    |
| saffron.finance                      | sfi                     |
| Perpetual Protocol                   | perp                    |
| BarnBridge                           | bond                    |
| CUDOS                                | cudos                   |
| Bonfida                              | fida                    |
| Frax                                 | frax                    |
| Frax Share                           | fxs                     |
| Juventus Fan Token                   | juv                     |
| Linear                               | lina                    |
| Mdex                                 | mdx                     |
| Mirror Protocol                      | mir                     |
| Marlin                               | pond                    |
| Paris Saint-Germain Fan Token        | psg                     |
| REVV                                 | revv                    |
| Rook                                 | rook                    |
| Trust Wallet Token                   | twt                     |
| ZKSpace                              | zks                     |
| Flow                                 | flow                    |
| Stratis                              | strax                   |
| Reef                                 | reef                    |
| Bitcoin Standard Hashrate Token      | btcst                   |
| The Sandbox                          | sand                    |
| SafePal                              | sfp                     |
| SKALE Network                        | skl                     |
| Phala Network                        | pha                     |
| WOO Network                          | woo                     |
| Raydium                              | ray                     |
| Akash Network                        | akt                     |
| Alchemix                             | alcx                    |
| DAO Maker                            | dao                     |
| DerivaDAO                            | ddx                     |
| Inverse Finance                      | inv                     |
| MAPS                                 | maps                    |
| Mask Network                         | mask                    |
| BENQI                                | qi                      |
| Radicle                              | rad                     |
| Rally                                | rly                     |
| SuperFarm                            | super                   |
| Tornado Cash                         | torn                    |
| AIOZ Network                         | aioz                    |
| Alpaca Finance                       | alpaca                  |
| Anchor Protocol                      | anc                     |
| Boson Protocol                       | boson                   |
| Convergence                          | conv                    |
| Fei USD                              | fei                     |
| Flux                                 | flux                    |
| Project Galaxy                       | gal                     |
| Illuvium                             | ilv                     |
| JasmyCoin                            | jasmy                   |
| Rai Reflex Index                     | rai                     |
| Alien Worlds                         | tlm                     |
| Tribe                                | tribe                   |
| Symbol                               | xym                     |
| Internet Computer                    | icp                     |
| Shiba Inu                            | shib                    |
| Somnium Space Cubes                  | cube                    |
| Dogelon Mars                         | elon                    |
| Ampleforth Governance Token          | forth                   |
| Gitcoin                              | gtc                     |
| Liquity                              | lqty                    |
| Media Network                        | media                   |
| APENFT                               | nft                     |
| QuickSwap                            | quick                   |
| Rari Governance Token                | rgt                     |
| Songbird                             | sgb                     |
| Step Finance                         | step                    |
| Persistence                          | xprt                    |
| Liquidity USD                        | lusd                    |
| Lido DAO                             | ldo                     |
| BitDAO                               | bit                     |
| Coin98                               | c98                     |
| Tranchess                            | chess                   |
| CLV                                  | clv                     |
| Covalent                             | cqt                     |
| Convex Finance                       | cvx                     |
| Dvision Network                      | dvi                     |
| Gala                                 | gala                    |
| Goldfinch                            | gfi                     |
| MOBOX                                | mbox                    |
| Moonriver                            | movr                    |
| PlayDapp                             | pla                     |
| Qredo                                | qrdo                    |
| RadioCaca                            | raca                    |
| SuperRare                            | rare                    |
| Shiden Network                       | sdn                     |
| SOMESING                             | ssx                     |
| StarLink                             | starl                   |
| Wrapped NCG                          | wncg                    |
| eCash                                | xec                     |
| Yield Guild Games                    | ygg                     |
| Pax Dollar                           | usdp                    |
| My Neighbor Alice                    | alice                   |
| ASD                                  | asd                     |
| XDC Network                          | xdc                     |
| Mina                                 | mina                    |
| Adventure Gold                       | agld                    |
| Star Atlas DAO                       | polis                   |
| dYdX                                 | dydx                    |
| Spell Token                          | spell                   |
| Ariva                                | arv                     |
| Assemble Protocol                    | asm                     |
| AstroSwap                            | astro                   |
| Star Atlas                           | atlas                   |
| BinaryX                              | bnx                     |
| Braintrust                           | btrst                   |
| Floki Inu                            | floki                   |
| Gods Unchained                       | gods                    |
| Highstreet                           | high                    |
| JOE                                  | joe                     |
| Moss Carbon Credit                   | mco2                    |
| Marinade Staked SOL                  | msol                    |
| Olympus                              | ohm                     |
| Orca                                 | orca                    |
| Ribbon Finance                       | rbn                     |
| Samoyedcoin                          | samo                    |
| Saber                                | sbr                     |
| Tokemak                              | toke                    |
| Wrapped Centrifuge                   | wcfg                    |
| Mines of Dalarnia                    | dar                     |
| Ethereum Name Service                | ens                     |
| GYEN                                 | gyen                    |
| Immutable X                          | imx                     |
| KOK                                  | kok                     |
| Boba Network                         | boba                    |
| Merit Circle                         | mc                      |
| Maple                                | mpl                     |
| ConstitutionDAO                      | people                  |
| BitTorrent (new)                     | bttc                    |
| Vulcan Forged PYR                    | pyr                     |
| Tether EURt                          | eurt                    |
| Casper                               | cspr                    |
| Automata Network                     | ata                     |
| ApeCoin                              | ape                     |
| LooksRare                            | looks                   |
| Moonbeam                             | glmr                    |
| Tulip Protocol                       | tulip                   |
| STEPN                                | gmt                     |
| Biconomy                             | bico                    |
| Alpine F1 Team Fan Token             | alpine                  |
| Astar                                | astr                    |
| PowerPool                            | cvp                     |
| Gari Network                         | gari                    |
| Optimism                             | op                      |
| SHPING                               | shping                  |
| Stargate Finance                     | stg                     |
| Voxies                               | voxel                   |
| Zebec Protocol                       | zbc                     |
| Acala Token                          | aca                     |
| Bounce Finance Governance Token      | auction                 |
| Eden                                 | eden                    |
| League of Kingdoms Arena             | loka                    |
| MetisDAO                             | metis                   |
| Ooki Protocol                        | ooki                    |
| Pundi X                              | pundix                  |
| Threshold                            | t                       |
| Voyager Token                        | vgx                     |
| USDD                                 | usdd                    |
| Chia                                 | xch                     |
| Staked Ether Lido                    | steth                   |
| poundtoken                           | gbpt                    |
| Terra 2.0                            | luna2                   |
| Chain                                | xcn                     |
| NYM                                  | nym                     |
| Efinity Token                        | efi                     |
| WEMIX                                | wemix                   |
| Step App                             | fitfi                   |
| Sweat Economy                        | sweat                   |
| EthereumPoW                          | ethw                    |

## Appendix B

The following table lists the weights applied to each one-minute time interval described in Section 5.4 Calculation Algorithm.

| Time Interval | Weight   |
| ------------- | -------- |
| 0             | 0.000000 |
| 1             | 0.000526 |
| 2             | 0.001052 |
| 3             | 0.001578 |
| 4             | 0.002104 |
| 5             | 0.002630 |
| 6             | 0.003156 |
| 7             | 0.003682 |
| 8             | 0.004208 |
| 9             | 0.004734 |
| 10            | 0.005260 |
| 11            | 0.005786 |
| 12            | 0.006312 |
| 13            | 0.006838 |
| 14            | 0.007364 |
| 15            | 0.007890 |
| 16            | 0.008416 |
| 17            | 0.008942 |
| 18            | 0.009468 |
| 19            | 0.009994 |
| 20            | 0.010520 |
| 21            | 0.011046 |
| 22            | 0.011572 |
| 23            | 0.012098 |
| 24            | 0.012624 |
| 25            | 0.013150 |
| 26            | 0.013676 |
| 27            | 0.014202 |
| 28            | 0.014728 |
| 29            | 0.015254 |
| 30            | 0.015780 |
| 31            | 0.016306 |
| 32            | 0.016832 |
| 33            | 0.017358 |
| 34            | 0.017884 |
| 35            | 0.018410 |
| 36            | 0.018936 |
| 37            | 0.019462 |
| 38            | 0.019988 |
| 39            | 0.020514 |
| 40            | 0.021040 |
| 41            | 0.021566 |
| 42            | 0.022092 |
| 43            | 0.022618 |
| 44            | 0.023144 |
| 45            | 0.023670 |
| 46            | 0.024196 |
| 47            | 0.024722 |
| 48            | 0.025248 |
| 49            | 0.025774 |
| 50            | 0.026300 |
| 51            | 0.026826 |
| 52            | 0.027352 |
| 53            | 0.027878 |
| 54            | 0.028404 |
| 55            | 0.028930 |
| 56            | 0.029456 |
| 57            | 0.029982 |
| 58            | 0.030508 |
| 59            | 0.050000 |
| 60            | 0.050000 |
