---
title: CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: CreateItem 要素は、Exchange ストア内のアイテムを作成するための要求を定義します。
ms.openlocfilehash: 235664b7baeceeccb14135fd346123f0f7d99346
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527062"
---
# <a name="createitem"></a>CreateItem

**CreateItem**要素は、Exchange ストア内のアイテムを作成するための要求を定義します。 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

**CreateItemType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|属性|説明|
|:-----|:-----|
|**MessageDisposition** <br/> |アイテムが作成された後に処理される方法について説明します。 電子メールメッセージの属性は必須です。 この属性は、電子メールメッセージにのみ適用されます。  <br/> |
|**Send会議の招待** <br/> |会議出席依頼が作成された後に処理される方法について説明します。 この属性は、予定表アイテムに必要です。  <br/> |
   
#### <a name="messagedisposition-attribute"></a>MessageDisposition 属性

|値|説明|
|:-----|:-----|
|SaveOnly  <br/> |メッセージアイテムは、 [SavedItemFolderId](saveditemfolderid.md)要素によって指定されたフォルダーに保存されます。 メッセージは、 [SendItem 操作](senditem-operation.md)を使用して後で送信できます。 アイテム識別子が応答で返されます。 アイテムの識別子は、メッセージアイテム以外のアイテムの種類に対しては返されません。 これには、応答オブジェクトが含まれます。  <br/> |
|SendOnly  <br/> |アイテムは送信されますが、[送信済みアイテム] フォルダーにコピーは保存されません。 応答では、アイテム識別子は返されません。<br/><br/>**注**: このオプションでは宛先フォルダーを指定できないため、 **CreateItem**は、sendonly オプションが使用されている場合は代理人アクセスをサポートしていません。 回避策として、アイテムを作成し、アイテム識別子を取得してから、SendItem 操作を使用してアイテムを送信します。           |
|SendAndSaveCopy  <br/> |アイテムが送信され、 [SavedItemFolderId](saveditemfolderid.md)要素によって識別されるフォルダーにコピーが保存されます。 応答では、アイテム識別子は返されません。<br/><br/>**注**: 会議出席依頼は、 [SavedItemFolderId](saveditemfolderid.md)プロパティによって指定されたフォルダーには保存されません。 予定表の場合、 **SavedItemFolderId**プロパティで指定できるのは、予定表アイテムの保存場所のみです。 会議出席依頼アイテムが保存される場所を制御することはできません。 関連付けられた予定表アイテムのみがコピーされ、 **SavedItemFolderId**プロパティによって識別されるフォルダーに保存されます。           |
   
#### <a name="sendmeetinginvitations-attribute"></a>Send会議の招待の属性

|値|説明|
|:-----|:-----|
|SendToNone  <br/> |アイテムが会議出席依頼の場合、予定表アイテムとして保存されますが、送信されません。  <br/> |
|SendOnlyToAll  <br/> |会議出席依頼はすべての出席者に送信されますが、[送信済みアイテム] フォルダーには保存されません。  <br/> |
|SendToAllAndSaveCopy  <br/> |会議出席依頼はすべての出席者に送信され、 [SavedItemFolderId](saveditemfolderid.md)要素によって識別されるフォルダーにコピーが保存されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|要素|説明|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |新しいアイテムを作成できるターゲットフォルダーを指定します。 **MessageDisposition**属性が sendonly に設定されている場合は、作成されたメッセージのみが送信されます。 このメッセージは、 [SavedItemFolderId](saveditemfolderid.md)要素によって識別されるフォルダーには配置されません。  <br/> |
|[アイテム (非 Emptyarrayofallitemstype)](items-nonemptyarrayofallitemstype.md) <br/> |[SavedItemFolderId](saveditemfolderid.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [CreateItemResponse](createitemresponse.md)  
- [CreateItem 操作](createitem-operation.md)
- [電子メールメッセージの作成](https://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [連絡先の作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [タスクの作成](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [予定の作成](https://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

