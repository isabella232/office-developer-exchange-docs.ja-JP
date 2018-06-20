---
title: NetworkRequirements (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: NetworkRequirements 要素には、クライアント コンピューターがネットワークでサーバーに接続するインターネット サービス プロバイダー (ISP) の要件を満たしているかどうかを使用する基準が含まれています。
ms.openlocfilehash: f3abcff04cd4121b8dcc7ceff7658ad389e6d0b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832529"
---
# <a name="networkrequirements-pox"></a>NetworkRequirements (POX)

**NetworkRequirements**要素には、クライアント コンピューターがネットワークでサーバーに接続するインターネット サービス プロバイダー (ISP) の要件を満たしているかどうかを使用する基準が含まれています。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[NetworkRequirements (POX)](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[IPv4Start (POX)](ipv4start-pox.md) <br/> |範囲の IP バージョン 4 (IPv4) の開始を示すものを使用して、ネットワーク上のコンピューターを識別するアドレスです。  <br/> |
|[IPv4End (POX)](ipv4end-pox.md) <br/> |範囲の IP バージョン 4 (IPv4) の終了位置を示すアドレス、ネットワーク上のコンピューターを識別するために使用します。  <br/> |
|[IPv6Start (POX)](ipv6start-pox.md) <br/> |範囲の IP バージョン 6 (IPv6) の開始を示すものを使用して、ネットワーク上のコンピューターを識別するアドレスです。  <br/> |
|[IPv6End (POX)](ipv6end-pox.md) <br/> |範囲の IP バージョン 6 (IPv6) の終了位置を示す、ネットワーク上のコンピューターの識別に使用されるアドレスです。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

電子メール クライアントがネットワークの要件に一致しない場合は、他のプロトコルの種類にしてください。 Isp は、ISP のネットワーク上にある認証を必要としないが、必要な[プロトコル (POX)](protocol-pox.md)タグを持つサーバーの 1 つのセットを提供することができます。 Isp には、認証を必要とするが、特定のネットワーク上に存在する必要はありませんサーバーの別のセットが一覧表示します。 
  
**NetworkRequirements**要素は、オプションです。 
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

