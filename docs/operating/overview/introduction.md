---
title: Operate a Neon Proxy
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

*This guide is for people who want to register with Neon EVM as a proxy operator for processing transactions on Solana. It is assumed the reader has prior experience compiling Solana-based blockchain nodes, or has worked as blockchain validators.*

## Introduction
Ethereum users have the opportunity to run their smart contract-based applications on Solana via Neon EVM. Smart contracts generate transactions in accordance with the Ethereum rules and submit them to Neon EVM. Since the structures of Ethereum and Solana transactions differ from each other, Neon EVM contains special proxy servers that are responsible for converting and executing transactions in Solana. These servers are configured and maintained by Neon EVM proxy operators.

This guide contains a list of the proxy operator's duties, as well as instructions to ensure the successful operation of a proxy and the successful execution of transactions.

## Duties of a Proxy Operator
A proxy operator's main task is to install software on a server in order to accept a transaction formed according to Ethereum rules, and to ensure its execution in Solana. This involves:
 * Configuring a proxy server to perform the following operations:
    * Receiving requests over Web3 API protocol
    * Shaping responses using Web3 API protocol
    * Converting transactions to the Solana format
 * Connecting a proxy server to a Solana cluster RPC endpoint
 * Successfully executing transactions

:::note
All operations related to the execution of transactions on Solana are performed by the software installed on your node.
:::

## Proxy Requirements

There are three ways:
1. Basic
2. Enhanced
3. Enterprise

Please make sure you have hardware that meets the corresponding requirements before proceeding:

<Tabs>
  <TabItem value="basic" label="Basic" default>

|Component|Requirement                           |
|-----|:-----------------------------------------|
|Operating System | Linux (Ubuntu/CentOS recommended) |
|CPU | 4 vCPU |
|RAM | 8 GB |
|Storage | 500 GB |
  </TabItem>
  <TabItem value="enhanced" label="Enhanced">

|Component|Requirement                           |
|-----|:-----------------------------------------|
|Servers/VMs | At least two (2) with Intel Processor x86_64 |
|CPU | 16 vCPU (for each server/VM) |
|RAM | 32 GB (for each server/VM) |
|Storage | 1 TB |
  </TabItem>
    <TabItem value="enterprise" label="Enterprise">
    Depends on your infrastructure and expected outcome.
  </TabItem>
</Tabs>