---
title: 内部 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 69c22546-ebd6-4a03-b0b4-bbac72ec5551
description: Internal 要素には、クライアントが組織のネットワーク内からExchangeに接続するために使用できる URL のコレクションが含まれる。
ms.openlocfilehash: f87c5e21eff87965c9b6ff6f3d59e2b3a37b87f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541120"
---
# <a name="internal-pox"></a>内部 (POX)

**Internal 要素** には、クライアントが組織のネットワーク内からネットワークに接続するために使用Exchange URL のコレクションが含まれる。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[内部 (POX)](internal-pox.md)
  
```xml
<Internal>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</Internal>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[OWAUrl (POX)](owaurl-pox.md) <br/> |Web Access をホストするクライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行している特定のコンピューターにアクセスするために使用される URL と認証スキーマOutlookします。  <br/> |
|[Protocol (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされているクライアントを実行しているコンピューター Microsoft Exchange Server接続するための仕様が含まれている。 この **Protocol** 要素には、接続プロトコルを指定する [Type (POX)](type-pox.md) 要素と、可用性 Web サービスの EWS エンドポイントを指定する [ASUrl (POX)](asurl-pox.md) 要素の 2 つの子要素があります。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーの役割がインストールされているクライアントを実行しているコンピューター Microsoft Exchange Server接続するための仕様が含まれている。  <br/> |
   
## <a name="remarks"></a>注釈

**Internal 要素** は、Protocol 要素の省略可能な子 **要素** です。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

