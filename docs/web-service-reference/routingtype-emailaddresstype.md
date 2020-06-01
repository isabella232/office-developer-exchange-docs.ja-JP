---
title: RoutingType (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 683216be-9972-4f48-a148-c34bfe7f53e5
description: RoutingType 要素は、メールボックスのアドレスの種類を定義します。
ms.openlocfilehash: d4229f2857a5c99cc9bb7ff9b9b103de099a0055
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465087"
---
# <a name="routingtype-emailaddresstype"></a>RoutingType (EmailAddressType)

**Routingtype**要素は、メールボックスのアドレスの種類を定義します。 
  
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
|[ActingAs](actingas.md) <br/> |発信者が送信者として送信しているユーザーを識別します。  <br/> |
|[メールボックス](mailbox.md) <br/> |完全に解決された電子メールアドレスを識別します。  <br/> |
|[RoomList](roomlist.md) <br/> |会議室のリストを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、ルーティングの種類を表します。 SMTP は、この要素の通常のテキスト値です。
  
## <a name="remarks"></a>注釈

この要素は、 [Mailbox](mailbox.md)要素では省略可能です。 別の[Routingtype (EmailAddress)](routingtype-emailaddress.md)要素は、可用性の操作に使用されます。 
  
この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

