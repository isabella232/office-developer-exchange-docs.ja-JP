---
title: AddressBook (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: AddressBook 要素には、MAPI/HTTP プロトコルを使用してクライアントをアドレス帳サーバーに接続するための仕様が含まれている。
ms.openlocfilehash: 28de1d41146b082c8b7f82c868fbbed1ce2c483e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546799"
---
# <a name="addressbook-pox"></a>AddressBook (POX)

**AddressBook 要素には**、MAPI/HTTP プロトコルを使用してクライアントをアドレス帳サーバーに接続するための仕様が含まれている。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[AddressBook (POX)](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |MAPI/HTTP プロトコルを使用して組織のネットワーク外からアドレス帳にアクセスするために使用する URL が含まれる。  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |MAPI/HTTP プロトコルを使用して組織のネットワーク内からアドレス帳にアクセスするために使用する URL が含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |クライアントをクライアント アクセス サーバーに接続するための仕様が含まれる。  <br/> |
   
## <a name="remarks"></a>注釈

**AddressBook 要素** は、Type 属性値 [が "mapiHttp" の Protocol (POX)](protocol-pox.md)要素を持つ応答に存在します。  
  
**AddressBook** 要素は、ビルド Exchange Online 15.00.0847.032 (Exchange Server 2013 SP1) から始まる Office 365 の一部として MAPI/HTTP プロトコルとターゲット Exchange Online、および Exchange のオンプレミス バージョンを実装するクライアントで使用できます。 
  
## <a name="see-also"></a>関連項目

- [POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

