---
description: Join a Hedera Testnet
---

# Testnets

## Overview

Hedera testnets provides developers with access to a free testing environment for Hedera network services. Testnets simulate the exact same devlopment environment as you would expect for mainnet. This includes transaction fees, throttles, available services, etc. Once your application has been built and tested in this test enviornment you can expect to migrate your decentralized application to mainnet without any changes. Testnets are likely to change and data may be deleted

**Test Networks:**

| **Name** | Description |
| :--- | :--- |
| **Test Network** | Runs the same code as the Hedera mainnet, designed to provide a pre-production environment for developers about to move to mainnet. You can find compatible SDKs [here](../docs/sdks/#hedera-supported-sdks). |
| **Preview Test Network** | Code that is under development by the Hedera team, and likely to be used in an upcoming release, designed to give developers early exposure to features coming down the pipe. Updates to the network are made frequently. There is no guarentee a SDK will readily support the up and coming features.  |

{% hint style="warning" %}
**Limited Support**  
Transactions are currently throttled for mainnet and testnet. You will receive a "BUSY" response if the number of transactions submitted to the network exceeds the threshold value.
{% endhint %}

| Network Service | Availability  |
| :--- | :--- |
| Cryptocurrency | Limited |
| Smart Contracts | Limited |
| File Service | Limited |
| Consensus Service | Limited  |

#### Network Throttles

<table>
  <thead>
    <tr>
      <th style="text-align:left">Network Request Type</th>
      <th style="text-align:left">Throttle (tps)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Cryptocurrency Transactions</td>
      <td style="text-align:left">
        <p>CryptoTransfer transactions: 10,000 tps</p>
        <p>All other cryptocurrency transactions<b>: </b>13 tps</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Consensus Transactions</td>
      <td style="text-align:left">
        <p>MessageSubmit transactions: 1,000 tps
          <br />createTopic: 5tps</p>
        <p>getTopicInfo/updateTopic/deleteTopic: 100 tps</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">File Transactions</td>
      <td style="text-align:left">All transaction types: 13 tps</td>
    </tr>
    <tr>
      <td style="text-align:left">Smart Contract Transactions</td>
      <td style="text-align:left">All transaction types: 13 tps</td>
    </tr>
    <tr>
      <td style="text-align:left">Queries</td>
      <td style="text-align:left">6,500 tps</td>
    </tr>
    <tr>
      <td style="text-align:left">Receipts</td>
      <td style="text-align:left">unlimited (no throttle)</td>
    </tr>
  </tbody>
</table>

