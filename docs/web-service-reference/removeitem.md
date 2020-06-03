---
title: RemoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveItem
api_type:
- schema
ms.assetid: 766878e3-9007-454f-8501-45139bc5c0e2
description: RemoveItem 要素は、会議の取り消しメッセージが受信されたときに会議アイテムを削除するために使用される response オブジェクトを表します。
ms.openlocfilehash: c0cd5c1f9894287ee78c2f7a65b8f4d3b943414e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467691"
---
# <a name="removeitem"></a>RemoveItem

**Removeitem**要素は、会議の取り消しメッセージが受信されたときに会議アイテムを削除するために使用される response オブジェクトを表します。 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 **RemoveItemType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ObjectName** <br/> |RemoveItem reply オブジェクトクラスの名前を英語の文字列として表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ReferenceItemId](referenceitemid.md) <br/> |RemoveItem response オブジェクトが参照するアイテムを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アイテム (非 Emptyarrayofallitemstype)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。  <br/> |
   
## <a name="remarks"></a>注釈

 **Removeitem**は、[会議の取り消し](meetingcancellation.md)に対してのみ有効です。 それ以外の場合は、エラーがスローされます。
  
> [!NOTE]
> 会議のキャンセルの[Itemclass](itemclass.md)は IPM です。予約を取り消しました。 
  
[会議の要求](meetingrequest.md)および関連付けられた予定表[アイテム](calendaritem.md)を削除するには、 **Removeitem**ではなく、 [declineitem](declineitem.md) response オブジェクトを使用します。
  
 **Removeitem**は、代理人アクセスをサポートしていません。 
  
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

