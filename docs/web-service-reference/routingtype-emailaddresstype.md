---
title: RoutingType (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 683216be-9972-4f48-a148-c34bfe7f53e5
description: RoutingType 要素は、メールボックスのアドレスの種類を定義します。
ms.openlocfilehash: fdbe40bd74debe517739e0fe0c47ed108bd614c6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509369"
---
# <a name="routingtype-emailaddresstype"></a>RoutingType (EmailAddressType)

**RoutingType 要素** は、メールボックスのアドレスの種類を定義します。 
  
```XML
<RoutingType/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |呼び出し元が送信するユーザーを識別します。  <br/> |
|[メールボックス](mailbox.md) <br/> |完全に解決された電子メール アドレスを識別します。  <br/> |
|[RoomList](roomlist.md) <br/> |会議室の一覧を識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ルーティングの種類を表します。 SMTP は、この要素の一般的なテキスト値です。
  
## <a name="remarks"></a>注釈

この要素は [、Mailbox 要素では省略](mailbox.md) 可能です。 可用性 [操作には、別の RoutingType (EmailAddress)](routingtype-emailaddress.md) 要素が使用されます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

