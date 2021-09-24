---
title: NetworkRequirements (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: NetworkRequirements 要素には、クライアント コンピューターがサーバーに接続するためのインターネット サービス プロバイダー (ISP) の要件を満たすネットワーク上にあるかどうかを判断するために使用される条件が含まれます。
ms.openlocfilehash: 07a258ad48b74c614ce367db0f893ed884cf3f75
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509516"
---
# <a name="networkrequirements-pox"></a>NetworkRequirements (POX)

**NetworkRequirements** 要素には、クライアント コンピューターがサーバーに接続するためのインターネット サービス プロバイダー (ISP) の要件を満たすネットワーク上にあるかどうかを判断するために使用される条件が含まれます。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[NetworkRequirements (POX)](networkrequirements-pox.md)
  
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
|[IPv4Start (POX)](ipv4start-pox.md) <br/> |ネットワーク上のコンピューターを識別するために使用される IP バージョン 4 (IPv4) アドレスの範囲の開始を識別します。  <br/> |
|[IPv4End (POX)](ipv4end-pox.md) <br/> |ネットワーク上のコンピューターを識別するために使用される IP バージョン 4 (IPv4) アドレスの範囲の終了を識別します。  <br/> |
|[IPv6Start (POX)](ipv6start-pox.md) <br/> |ネットワーク上のコンピューターを識別するために使用される IP バージョン 6 (IPv6) アドレスの範囲の開始を識別します。  <br/> |
|[IPv6End (POX)](ipv6end-pox.md) <br/> |ネットワーク上のコンピューターを識別するために使用される IP バージョン 6 (IPv6) アドレスの範囲の終了を識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされている 2007 年Microsoft Exchange Serverコンピューターにクライアントを接続するための仕様が含まれている。  <br/> |
   
## <a name="remarks"></a>注釈

電子メール クライアントがネットワーク要件と一致しない場合は、他のプロトコルの種類を試してください。 ISP は、認証を必要としないが ISP ネットワーク上にある必要があるプロトコル [(POX)](protocol-pox.md) タグを持つ 1 セットのサーバーを提供する場合があります。 ISP は、認証を必要とするが、特定のネットワーク上にいる必要はない別のサーバー セットを一覧表示できます。 
  
**NetworkRequirements 要素** はオプションです。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

