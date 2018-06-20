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
description: AttendeeType 要素は、電子メール (EmailAddressType) の要素で指定されている参加者の種類を表します。 この要素は、推奨事項を満たすため、要求で使用されます。
ms.openlocfilehash: a08532ed78296102ee252c1e0c40beee7ca8ea5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759462"
---
# <a name="attendeetype"></a>AttendeeType

**AttendeeType**要素は、[電子メール (EmailAddressType)](email-emailaddresstype.md)の要素で指定されている参加者の種類を表します。 この要素は、推奨事項を満たすため、要求で使用されます。 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
- [AttendeeType](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 **MeetingAttendeeType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |個々 のメールボックス ユーザーのメールボックスのユーザーに返されるデータの種類のオプションを表します。  <br/> 以下は、この要素の XPath です。  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、この要素の必要があります。 次の表は、この要素の有効な値を一覧します。
  
|**値**|**説明**|
|:-----|:-----|
|Organizer  <br/> |メールボックス ユーザーと出席者の予定表アイテムを作成しました。  <br/> |
|必須  <br/> |必須の出席者、会議には、メールボックス ・ ユーザーです。  <br/> |
|省略可能  <br/> |任意の出席者、会議には、メールボックス ・ ユーザーです。  <br/> |
|ルーム  <br/> |メールボックスを表すエンティティ部屋リソースが、会議に使用します。  <br/> |
|リソース  <br/> |テレビ会議で使用するためにスケジュールされている最初のプロジェクターなどのリソースです。  <br/> |
   
## <a name="remarks"></a>備考

この要素は、 [MailboxData](mailboxdata.md)要素の必須の子要素です。 この要素はことができます[MailboxData](mailboxdata.md)要素内で 1 回のみ発生します。 この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割を持つ MicrosoftExchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。 
  
> [!NOTE]
> AttendeeType スキーマの種類が使用され、出席者の予定表アイテムを表します。 AttendeeType スキーマの種類の要素にこの要素を混同しないでください。 
  
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

