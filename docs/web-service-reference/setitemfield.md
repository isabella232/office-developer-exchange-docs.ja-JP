---
title: SetItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetItemField
api_type:
- schema
ms.assetid: 85284fcb-bd1e-4fda-9dab-cb4cd637cd5b
description: SetItemField 要素は、UpdateItem 操作内の項目の 1 つのプロパティへの更新プログラムを表します。
ms.openlocfilehash: 012e6ae21af653b4bf12588e5a97334a62884059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833439"
---
# <a name="setitemfield"></a>SetItemField

**SetItemField**要素は、 [UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティへの更新プログラムを表します。
  
```xml
<SetItemField>
   <FieldURI/>
   <Item/>
</SetItemField>
```

 **SetItemFieldType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々 のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |設定するのには、拡張 MAPI プロパティを識別します。  <br/> |
|[アイテム](item.md) <br/> |Exchange ストア内の項目を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |更新する Exchange 電子メール メッセージを表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |更新するのには、Exchange 予定表のアイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange 連絡先を更新する項目を表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |更新する配布リストを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |会議を更新するメッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |更新する会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |更新するのには会議の返信を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |更新するのには、会議の取り消し通知を表します。  <br/> |
|[タスク](task.md) <br/> |更新するタスクを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[更新 (アイテム)](updates-item.md) <br/> |定義する要素のセットが含まれていて、このオプションを設定すると、アイテムのプロパティの変更を削除します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [UpdateItem 操作](updateitem-operation.md)

