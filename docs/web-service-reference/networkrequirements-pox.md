---
title: NetworkRequirements 要件 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: NetworkRequirements 要件要素には、サーバーに接続するためにインターネットサービスプロバイダー (ISP) の要件を満たすネットワーク上にクライアントコンピューターがあるかどうかを判断するために使用される条件が含まれています。
ms.openlocfilehash: d588f7eb12a445fba9c997c4b9db0a6842105b4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462725"
---
# <a name="networkrequirements-pox"></a>NetworkRequirements 要件 (POX)

**Networkrequirements 要件**要素には、サーバーに接続するためにインターネットサービスプロバイダー (ISP) の要件を満たすネットワーク上にクライアントコンピューターがあるかどうかを判断するために使用される条件が含まれています。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[NetworkRequirements 要件 (POX)](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[IPv4Start (POX)](ipv4start-pox.md) <br/> |ネットワーク上のコンピューターを識別するために使用される IP version 4 (IPv4) アドレスの範囲の開始を識別します。  <br/> |
|[IPv4End (POX)](ipv4end-pox.md) <br/> |ネットワーク上のコンピューターを識別するために使用される IP version 4 (IPv4) アドレスの範囲の末尾を識別します。  <br/> |
|[IPv6Start (POX)](ipv6start-pox.md) <br/> |ネットワーク上のコンピューターを識別するために使用される IP version 6 (IPv6) アドレスの範囲の開始を識別します。  <br/> |
|[IPv6End (POX)](ipv6end-pox.md) <br/> |ネットワーク上のコンピューターを識別するために使用される IP version 6 (IPv6) アドレスの範囲の末尾を識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="remarks"></a>注釈

電子メールクライアントがネットワーク要件を満たしていない場合は、他のプロトコルの種類を試す必要があります。 Isp は、認証を必要とせず、ISP ネットワーク上で必要な[プロトコル (POX)](protocol-pox.md)タグを備えたサーバーのセットを提供することがあります。 Isp は、認証を必要とする別のサーバーセットを一覧表示することができますが、特定のネットワークである必要はありません。 
  
**Networkrequirements 要件**要素はオプションです。 
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

