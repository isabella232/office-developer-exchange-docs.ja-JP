---
title: AppendToItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppendToItemField
api_type:
- schema
ms.assetid: 66dbcb4a-ae6d-4648-8610-67187bdb105c
description: AppendToItemField 要素は、UpdateItem 操作中に 1 つのアイテムのプロパティを追加するデータを識別します。
ms.openlocfilehash: b432399e84ee4a3fd7edc5d3f803079435c79143
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759338"
---
# <a name="appendtoitemfield"></a>AppendToItemField

**AppendToItemField**要素は、 [UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムのプロパティを追加するデータを識別します。
  
- [UpdateItem](updateitem.md)
  
- [ItemChanges](itemchanges.md)
  
- [ItemChange](itemchange.md)
  
- [更新 (アイテム)](updates-item.md)
  
- [AppendToItemField](appendtoitemfield.md)
  
```xml
<AppendToItemField>
   <FieldURI/>
   <Item/>
</AppendToItemField>
```

 **AppendToItemFieldType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々 のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |追加するのには、拡張 MAPI プロパティを識別します。  <br/> |
|[アイテム](item.md) <br/> |Exchange ストア内の項目を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メール メッセージを表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の返信を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消し通知を表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[更新 (アイテム)](updates-item.md) <br/> |定義する配列が含まれていて、このオプションを設定すると、アイテムのプロパティの変更を削除します。  <br/> この要素への XPath 式は、次のようにします。`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a>備考

特定のプロパティのサポートだけでは、操作を追加します。 追加することをサポートしていないプロパティを追加しようとするは、エラーになります。
  
更新操作の場合は、1 つの要求内で 1 つのプロパティを変更できます。 その 1 つのプロパティは、 [Path](path.md)要素に参照されなければなりません。 だけ、派生クラス内の**項目**要素では、**パス**要素を 1 つだけ、1 つのプロパティを格納できますし。 
  
> [!NOTE]
> [Path](path.md)要素は、抽象です。 [FieldURI](fielduri.md)、 [IndexedFieldURI](indexedfielduri.md)、または[ExtendedFieldURI](extendedfielduri.md)要素によってそれに置き換え 必要があります。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- 
  [UpdateItem 操作](updateitem-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

