---
title: ExternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: ExternalUrl 要素には、MAPI/HTTP プロトコルを使用して、クライアントをアドレス帳サーバーまたはユーザーのメールボックスに接続するための URL が含まれる。
ms.openlocfilehash: 90aaf9cabedba4ea89e0ed47da010245006407ba
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510074"
---
# <a name="externalurl-pox"></a>ExternalUrl (POX)

**ExternalUrl 要素** には、MAPI/HTTP プロトコルを使用して、クライアントをアドレス帳サーバーまたはユーザーのメールボックスに接続するための URL が含まれる。 
  
```XML
<ExternalUrl/>
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

テキスト値は、ユーザーの組織外からアドレス帳サーバーまたはユーザーのメールボックスにアクセスするために使用できる URL を表します。
  
## <a name="remarks"></a>注釈

**ExternalUrl 要素** は、Type 属性値 [が "mapiHttp" の Protocol (POX)](protocol-pox.md)要素を持つ応答に存在できます。  
  
**ExternalUrl** 要素は、ビルド 15.00.0847.032 (Exchange Server 2013 SP1) から、MAPI/HTTP プロトコルとターゲット Exchange Online、Exchange Online を Office 365 の一部として実装するクライアント、および Exchange のオンプレミス バージョンで使用できます。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

