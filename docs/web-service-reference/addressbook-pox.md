---
title: AddressBook (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: AddressBook 要素には、MAPI/HTTP プロトコルを使用してアドレス帳サーバーにクライアントを接続するための仕様が含まれています。
ms.openlocfilehash: 0967ac123cd3bb0086fd004ea0d0d37c08d2e037
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463637"
---
# <a name="addressbook-pox"></a>AddressBook (POX)

**AddressBook**要素には、MAPI/HTTP プロトコルを使用してアドレス帳サーバーにクライアントを接続するための仕様が含まれています。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
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
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |MAPI/HTTP プロトコルを使用して、組織のネットワークの外部からアドレス帳にアクセスするために使用する URL が含まれています。  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |MAPI/HTTP プロトコルを使用して、組織のネットワーク内からアドレス帳にアクセスするために使用する URL が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントをクライアントアクセスサーバーに接続するための仕様が含まれています。  <br/> |
   
## <a name="remarks"></a>注釈

**AddressBook**要素は、 **Type**属性の値が "Http" である[Protocol (POX)](protocol-pox.md)要素を持つ応答に存在します。 
  
**AddressBook**要素は、MAPI/HTTP プロトコルおよびターゲット exchange online の一部としての exchange Online、Office 365 の一部としての exchange online、およびビルド 15.00.0847.032 (exchange SERVER 2013 SP1) 以降のオンプレミスバージョンの exchange を実装するクライアントで使用できます。 
  
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

