---
title: AttendeeType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeType
api_type:
- schema
ms.assetid: 048043a8-dbad-45a0-97c8-4cad63d8898b
description: AttendeeType 要素は、Email (EmailAddressType) 要素で識別される出席者の種類を表します。 この要素は、会議提案の要求で使用されます。
ms.openlocfilehash: 104b9f38cc891310ecb47c0b47837a912ced6ab7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462298"
---
# <a name="attendeetype"></a>AttendeeType

**AttendeeType**要素は、 [Email (emailaddresstype)](email-emailaddresstype.md)要素で識別される出席者の種類を表します。 この要素は、会議提案の要求で使用されます。 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
- [AttendeeType](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 **MeetingAttendeeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |個々のメールボックスユーザー、およびメールボックスユーザーに関して返されるデータの種類のオプションを表します。  <br/> この要素の XPath を次に示します。  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a>テキスト値

この要素にはテキスト値が必要です。 次の表に、この要素で使用できる値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|開催者  <br/> |予定表アイテムを作成したメールボックスユーザーと出席者。  <br/> |
|必須  <br/> |会議の必須出席者であるメールボックスユーザー。  <br/> |
|オプション  <br/> |会議の任意出席者であるメールボックスユーザー。  <br/> |
|Room  <br/> |会議に使用される会議室リソースを表すメールボックスエンティティ。  <br/> |
|関連情報  <br/> |会議で使用するようにスケジュールされている、テレビやプロジェクターなどのリソース。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は、 [MailboxData](mailboxdata.md)要素の必須の子要素です。 この要素は、 [MailboxData](mailboxdata.md)要素内で1回だけ発生します。 この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。 
  
> [!NOTE]
> AttendeeType スキーマの種類は、予定表アイテムへの出席者を表すために使用されます。 この要素は、AttendeeType スキーマ型の要素と混同しないでください。 
  
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

