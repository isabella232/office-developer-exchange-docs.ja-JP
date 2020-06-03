---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: InternalUrl 要素には、MAPI/HTTP プロトコルを使用して、ユーザーの組織内からアドレス帳サーバーまたはユーザーのメールボックスにクライアントを接続するための URL が含まれています。
ms.openlocfilehash: 9c6ba621a681ec54d88089de6b7ae1eefdebc679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465577"
---
# <a name="internalurl-pox"></a>InternalUrl (POX)

**Internalurl**要素には、MAPI/HTTP プロトコルを使用して、ユーザーの組織内からアドレス帳サーバーまたはユーザーのメールボックスにクライアントを接続するための URL が含まれています。 
  
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
|[AddressBook (POX)](addressbook-pox.md) <br/> |MAPI/HTTP プロトコルを使用して、アドレス帳サーバーにクライアントを接続するための仕様が含まれています。  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |MAPI/HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、ユーザーの組織内からアドレス帳サーバーまたはユーザーのメールボックスにアクセスするために使用できる URL を表します。
  
## <a name="remarks"></a>注釈

**Internalurl**要素は、 **Type**属性の値が "Http" である[Protocol (POX)](protocol-pox.md)要素を持つ応答に存在できます。 
  
**Internalurl**要素は、MAPI/HTTP プロトコルおよびターゲット exchange online の一部としての exchange Online、Office 365 の一部としての exchange online、および build 15.00.0847.032 (exchange SERVER 2013 SP1) 以降のオンプレミスバージョンの exchange を実装するクライアントで利用できます。 
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

