---
title: MailStore (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: MailStore 要素には、MAPI または HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれています。
ms.openlocfilehash: 4c82c7b61752cf7d91287a3968f6c642f4943855
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832301"
---
# <a name="mailstore-pox"></a>MailStore (POX)

**MailStore**要素には、MAPI または HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれています。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[MailStore (POX)](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |MAPI または HTTP プロトコルを使用して組織のネットワークの外部からのユーザーのメールボックスにアクセスするために使用する URL が含まれています。  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |MAPI または HTTP プロトコルを使用して組織のネットワーク内からのユーザーのメールボックスへのアクセスに使用する URL が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアント アクセス サーバーにクライアントを接続するための仕様が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

**MailStore**要素は、"mapiHttp"の**型**の属性値を持つ[プロトコル (POX)](protocol-pox.md)要素を持つ応答に存在します。 
  
**MailStore**要素は、ターゲット Exchange Online では、Office 365 の一部として Exchange Online MAPI または HTTP プロトコルを実装するクライアントに使用し、設置型のバージョンの Exchange が始まる 15.00.0847.032 (Exchange Server 2013 SP1) を構築します。 
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

