---
title: AttendeeType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AttendeeType
api_type:
- schema
ms.assetid: 048043a8-dbad-45a0-97c8-4cad63d8898b
description: AttendeeType 要素は、Email (EmailAddressType) 要素で識別される出席者の種類を表します。 この要素は、会議の提案の要求で使用されます。
ms.openlocfilehash: 5bcec50fe6cccc3df48ca9615dbd0d9418211b4b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533935"
---
# <a name="attendeetype"></a>AttendeeType

**AttendeeType 要素** は、Email [(EmailAddressType)](email-emailaddresstype.md)要素で識別される出席者の種類を表します。 この要素は、会議の提案の要求で使用されます。 
  
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
|[MailboxData](mailboxdata.md) <br/> |個々のメールボックス ユーザーと、メールボックス ユーザーに関して返されるデータの種類のオプションを表します。  <br/> 次に、この要素の XPath を示します。  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a>テキスト値

この要素には、テキスト値が必要です。 次の表に、この要素に使用できる値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|Organizer  <br/> |予定表アイテムを作成したメールボックス ユーザーと出席者。  <br/> |
|必須かどうか  <br/> |会議に必要な出席者であるメールボックス ユーザー。  <br/> |
|オプション  <br/> |会議の任意の出席者であるメールボックス ユーザー。  <br/> |
|Room  <br/> |会議に使用される会議室リソースを表すメールボックス エンティティ。  <br/> |
|リソース  <br/> |会議で使用するようにスケジュールされているテレビやプロジェクターなどのリソース。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は [、MailboxData](mailboxdata.md) 要素の必須の子要素です。 この要素は、MailboxData 要素で [1 回だけ発生](mailboxdata.md) します。 この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの /EWS/ ディレクトリにあります。 
  
> [!NOTE]
> AttendeeType スキーマの種類は、予定表アイテムの出席者を表す場合に使用します。 この要素を AttendeeType スキーマ型の要素と混同して使用しない。 
  
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

