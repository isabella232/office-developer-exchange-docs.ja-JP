---
title: 外部 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8eed1f79-6eb3-4a88-80fb-d4edf9f34fda
description: External 要素には、クライアントが組織のネットワークの外部から Exchange に接続するために使用できる Url のコレクションが含まれています。
ms.openlocfilehash: 45d7e72c5a43c5c468c1edd303a5e5ea8c2cb62e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457971"
---
# <a name="external-pox"></a>外部 (POX)

**External**要素には、クライアントが組織のネットワークの外部から Exchange に接続するために使用できる url のコレクションが含まれています。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[外部 (POX)](external-pox.md)
  
```XML
<External>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</External>

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

**External**要素は、 **Protocol**要素のオプションの子要素です。 
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

