---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: InternalUrl 要素には、アドレス帳のサーバーまたはユーザーの組織内からのユーザーのメールボックスに MAPI または HTTP プロトコルを使用してクライアントを接続するための URL が含まれています。
ms.openlocfilehash: 3823236081961128b31bb2c0f563062897c55814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831950"
---
# <a name="internalurl-pox"></a>InternalUrl (POX)

**InternalUrl**要素には、アドレス帳のサーバーまたはユーザーの組織内からのユーザーのメールボックスに MAPI または HTTP プロトコルを使用してクライアントを接続するための URL が含まれています。 
  
```XML
<InternalUrl/>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アドレス帳 (POX)](addressbook-pox.md) <br/> |MAPI または HTTP プロトコルを使用してアドレス帳のサーバーにクライアントを接続するための仕様が含まれています。  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |MAPI または HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、アドレス帳のサーバーまたはユーザーの組織内からのユーザーのメールボックスへのアクセスに使用できる URL を表します。
  
## <a name="remarks"></a>備考

**InternalUrl**要素は、"mapiHttp"の**型**の属性値を持つ[プロトコル (POX)](protocol-pox.md)要素を持つ応答で使用できます。 
  
**InternalUrl**要素は、ターゲット Exchange Online では、Office 365 の一部として Exchange Online MAPI または HTTP プロトコルを実装するクライアントに使用し、設置型のバージョンの Exchange が始まる 15.00.0847.032 (Exchange Server 2013 SP1) を構築します。. 
  
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

