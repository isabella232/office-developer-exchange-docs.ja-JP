---
title: RoutingType (EmailAddress)
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
ms.assetid: 74d83198-0d9d-4c78-a2bc-9a671859ff37
description: RoutingType 要素は、受信者のルーティング プロトコルを表します。
ms.openlocfilehash: cc4d18ff9fa18f0ec2024f15cb6a3bd4199832de
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534430"
---
# <a name="routingtype-emailaddress"></a>RoutingType (EmailAddress)

**RoutingType 要素** は、受信者のルーティング プロトコルを表します。 
  
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
|[Email (EmailAddressType)](email-emailaddresstype.md) <br/> |MailboxData オブジェクトの電子メール アドレスを指定します。 この要素は [、GetUserAvailability 操作で使用されます](getuseravailability-operation.md)。  <br/><br/> 次に、この要素の XPath を示します。  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Mailbox (Availability)](mailbox-availability.md) <br/> | SetUserOofSettings または GetUserOofSettings 要求のメールボックス ユーザーを表します。  <br/><br/>  この要素の XPath 式を次に示します。 <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値はオプションです。 指定可能な値は次のいずれかです。

* SMTP
* EX

値が指定されている場合は、SMTP の既定値が使用されます。
  
## <a name="remarks"></a>注釈

この要素は、Email [(EmailAddressType) 要素で一度に発生する可能性](email-emailaddresstype.md) があります。 この要素は必須ではありません。 この要素は、将来のプロトコルを含める場合に存在します。 別 **の RoutingType** 要素は、ユーザーのメールボックス内のアイテムにアクセスするために使用されます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

