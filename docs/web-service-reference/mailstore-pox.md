---
title: MailStore (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: MailStore 要素には、MAPI/HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれている。
ms.openlocfilehash: 543bcb8df84904f2b70d6feeabf16d1cc021f3e5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511123"
---
# <a name="mailstore-pox"></a>MailStore (POX)

**MailStore 要素には**、MAPI/HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれている。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[MailStore (POX)](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |MAPI/HTTP プロトコルを使用して組織のネットワークの外部からユーザーのメールボックスにアクセスするために使用する URL が含まれる。  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |MAPI/HTTP プロトコルを使用して、組織のネットワーク内からユーザーのメールボックスにアクセスするために使用する URL を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |クライアントをクライアント アクセス サーバーに接続するための仕様が含まれる。  <br/> |
   
## <a name="remarks"></a>注釈

**MailStore 要素** は、Type 属性値 [が "mapiHttp" のプロトコル (POX)](protocol-pox.md)要素を持つ応答に存在します。  
  
**MailStore** 要素は、MAPI/HTTP プロトコルを実装し、Office 365 の一部として Exchange Online、Exchange Online、およびビルド 15.00.0847.032 (Exchange Server 2013 SP1) から始まる Exchange のオンプレミス バージョンを実装するクライアントで使用できます。 
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

