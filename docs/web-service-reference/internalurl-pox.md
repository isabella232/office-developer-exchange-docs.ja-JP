---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: InternalUrl 要素には、MAPI/HTTP プロトコルを使用して、ユーザーの組織内からアドレス帳サーバーまたはユーザーのメールボックスにクライアントを接続するための URL が含まれる。
ms.openlocfilehash: 4ce04743c7d0f260439849a02f8f6d389f6c83fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542197"
---
# <a name="internalurl-pox"></a>InternalUrl (POX)

**InternalUrl 要素** には、MAPI/HTTP プロトコルを使用して、ユーザーの組織内からアドレス帳サーバーまたはユーザーのメールボックスにクライアントを接続するための URL が含まれる。 
  
```XML
<InternalUrl/>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AddressBook (POX)](addressbook-pox.md) <br/> |MAPI/HTTP プロトコルを使用してクライアントをアドレス帳サーバーに接続するための仕様が含まれる。  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |MAPI/HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ユーザーの組織内からアドレス帳サーバーまたはユーザーのメールボックスにアクセスするために使用できる URL を表します。
  
## <a name="remarks"></a>注釈

**InternalUrl 要素** は、Type 属性値 [が "mapiHttp" の Protocol (POX)](protocol-pox.md)要素を持つ応答に存在できます。  
  
**InternalUrl** 要素は、ビルド 15.00.0847.032 (Exchange Server 2013 SP1) から始まる Office 365 の一部として MAPI/HTTP プロトコルとターゲット Exchange Online Exchange Online、Exchange Online、およびオンプレミス バージョンの Exchange を実装するクライアントで使用できます。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

