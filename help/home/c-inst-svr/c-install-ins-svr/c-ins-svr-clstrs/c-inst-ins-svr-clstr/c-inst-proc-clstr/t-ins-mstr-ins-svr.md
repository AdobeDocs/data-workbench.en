---
description: To use a cluster, you must designate one Insight Server in the cluster to act as the master Insight Server.
seo-description: To use a cluster, you must designate one Insight Server in the cluster to act as the master Insight Server.
seo-title: Installing the Master Insight Server
solution: Insight
title: Installing the Master Insight Server
uuid: fe918c88-6554-4f45-9b2c-af65cf57c623
index: y
internal: n
snippet: y
---

# Installing the Master Insight Server{#installing-the-master-insight-server}

To use a cluster, you must designate one Insight Server in the cluster to act as the master Insight Server.

 A client component such as [!DNL Insight] or [!DNL Report] connects to the master [!DNL Insight Server] at the beginning of a session. At subsequent points during the session, the client might connect to other [!DNL Insight Servers] in the cluster to perform a query. These subsequent connections between the client and the other [!DNL Insight Servers] in the cluster are brokered by the master [!DNL Insight Server] and are transparent to the client.

Besides brokering connections between a client and other [!DNL Insight Servers] in the cluster, the master [!DNL Insight Server] acts as the central administrative point for the entire cluster. When you administer a cluster, you update the master [!DNL Insight Server]. The administrative changes that you make on the master [!DNL Insight Server] are retrieved by the other [!DNL Insight Servers] in the cluster.

**To install the master [!DNL Insight Server]** 

1. Determine which machine will act as the master [!DNL Insight Server].
1. Install and configure [!DNL Insight Server] (typically, an [!DNL Insight Server] FSU) on this machine as described in [Insight Server](../../../../../../home/c-inst-svr/c-inst-svr.md#concept-c5c7e4288dcf44c8b2a61e40fae891c0).
1. Install [!DNL Insight] and configure a connection to the master [!DNL Insight Server] as described in the * [!DNL Insight] User Guide*.
