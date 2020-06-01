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
description: RoutingType 要素は、受信者のルーティングプロトコルを表します。
ms.openlocfilehash: 2193e72c38c687669f6e052b4d2526029aa89d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459035"
---
# <a name="routingtype-emailaddress"></a>RoutingType (EmailAddress)

**Routingtype**要素は、受信者のルーティングプロトコルを表します。 
  
```XML
<RoutingType/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[電子メール (EmailAddressType)](email-emailaddresstype.md) <br/> |MailboxData オブジェクトの電子メールアドレスを指定します。 この要素は、 [Getuseravailability 操作](getuseravailability-operation.md)で使用されます。  <br/><br/> この要素の XPath を次に示します。  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[メールボックス (可用性)](mailbox-availability.md) <br/> | SetUserOofSettings または GetUserOofSettings 要求のメールボックスユーザーを表します。  <br/><br/>  この要素の XPath 式は次のとおりです。 <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値はオプションです。 指定可能な値は次のいずれかです。

* SMTP
* 渡し

値が指定されていない場合は、SMTP の既定値が使用されます。
  
## <a name="remarks"></a>注釈

この要素は、 [email (EmailAddressType)](email-emailaddresstype.md)要素で最大で1回発生する可能性があります。 この要素は必須ではありません。 この要素は、将来のプロトコルを含めるために存在します。 ユーザーのメールボックス内のアイテムにアクセスするには、別の**Routingtype**要素を使用します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [ユーザーの空き時間情報の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

