---
title: RoutingType (EmailAddress)
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
ms.assetid: 74d83198-0d9d-4c78-a2bc-9a671859ff37
description: RoutingType 要素は、受信者のルーティング プロトコルを表します。
ms.openlocfilehash: a0a6cf312bcb1d4b4818a82bc8d8d3e3f33ad6f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833255"
---
# <a name="routingtype-emailaddress"></a>RoutingType (EmailAddress)

**RoutingType**要素は、受信者のルーティング プロトコルを表します。 
  
```XML
<RoutingType/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[電子メール (EmailAddressType)](email-emailaddresstype.md) <br/> |MailboxData オブジェクトの電子メール アドレスを指定します。 この要素は、 [GetUserAvailability の操作](getuseravailability-operation.md)で使用されます。  <br/><br/> 以下は、この要素の XPath です。  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[メールボックス (可用性)](mailbox-availability.md) <br/> | SetUserOofSettings または GetUserOofSettings の要求をメールボックスのユーザーを表します。  <br/><br/>  この要素への XPath 式は、次のように。 <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は省略可能です。 唯一の有効値は、SMTP です。 値が指定されていない場合は、SMTP のデフォルト値が使用されます。
  
## <a name="remarks"></a>備考

この要素は、最大で 1 回、[電子メール (EmailAddressType)](email-emailaddresstype.md)の要素で発生します。 この要素は必須ではありません。 将来のプロトコルのため、この要素が存在しています。 もう 1 つの**RoutingType**要素は、ユーザーのメールボックス内のアイテムへのアクセスに使用されます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

