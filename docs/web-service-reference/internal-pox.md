---
title: Internal (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 69c22546-ebd6-4a03-b0b4-bbac72ec5551
description: Internal 要素には、組織のネットワーク内から Exchange に接続するためにクライアントが使用できる Url のコレクションが含まれています。
ms.openlocfilehash: 8164a018a11f9bae9c3abcbfebf6cf0694ca4183
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465598"
---
# <a name="internal-pox"></a>Internal (POX)

**Internal**要素には、組織のネットワーク内から Exchange に接続するためにクライアントが使用できる url のコレクションが含まれています。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[Internal (POX)](internal-pox.md)
  
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
|[OWAUrl (POX)](owaurl-pox.md) <br/> |Outlook Web Access をホストするクライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行している特定のコンピューターにアクセスするために使用される URL と認証スキーマについて説明します。  <br/> |
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。 この**プロトコル**要素には、2つの子要素 (接続プロトコルを指定する[Type (POX)](type-pox.md)要素と、可用性 web サービスの EWS エンドポイントを指定する[asurl (POX)](asurl-pox.md)要素のみが含まれます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="remarks"></a>注釈

**Internal**要素は、 **Protocol**要素のオプションの子要素です。 
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

