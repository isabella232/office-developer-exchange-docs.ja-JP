---
title: MailboxData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxData
api_type:
- schema
ms.assetid: e9e3f50c-5a7b-49c7-a9ea-117959c08352
description: MailboxData 要素は、個々のメールボックスユーザー、およびメールボックスユーザーに関して返されるデータの種類のオプションを表します。
ms.openlocfilehash: bfcb8c01d40af81097c7d9868006fe9b7b5519d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467250"
---
# <a name="mailboxdata"></a>MailboxData

**MailboxData**要素は、個々のメールボックスユーザー、およびメールボックスユーザーに関して返されるデータの種類のオプションを表します。 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
```xml
<MailboxData>
   <Email>...</Email>
   <AttendeeType>...</AttendeeType>
   <ExcludeConflicts>...</ExcludeConflicts>
<MailboxData>
```

**MailboxData**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[電子メール (EmailAddressType)](email-emailaddresstype.md) <br/> |GetUserAvailability クエリのメールボックスユーザーを表します。  <br/> |
|[AttendeeType](attendeetype.md) <br/> |[Email (EmailAddressType)](email-emailaddresstype.md)要素で識別された出席者の種類を表します。 これは、会議提案の要求で使用されます。  <br/> |
|[ExcludeConflicts](excludeconflicts.md) <br/> |出席者間での予定表の時間について、提案された時間を返すかどうかを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MailboxDataArray](mailboxdataarray.md) <br/> |可用性情報を照会するメールボックスの一覧が含まれています。  <br/> この要素の XPath を次に示します。  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a>注釈

クライアントアプリケーションでは、1対多の**MailboxData**要素を定義できます。 
  
> [!NOTE]
> この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
## <a name="example"></a>例

```xml
<MailboxDataArray>
  <MailboxData xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
    <Email>
      <Name></Name>
      <Address>someone@ExServer.example.com</Address>
      <RoutingType>SMTP</RoutingType>
    </Email>
    <AttendeeType>Organizer</AttendeeType>
    <ExcludeConflicts>false</ExcludeConflicts>
  </MailboxData>
</MailboxDataArray>
```

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

