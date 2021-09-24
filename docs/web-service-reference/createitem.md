---
title: CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: CreateItem 要素は、カスタム ストアにアイテムを作成する要求をExchangeします。
ms.openlocfilehash: 7276b88bd3b90edc68d7ac8fd4a7646324eadb61
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526499"
---
# <a name="createitem"></a>CreateItem

**CreateItem 要素は**、アイテムストアにアイテムを作成する要求をExchangeします。 
  
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
|**MessageDisposition** <br/> |作成後のアイテムの処理方法について説明します。 この属性は、電子メール メッセージに必要です。 この属性は、電子メール メッセージにのみ適用されます。  <br/> |
|**SendMeetingInvitations** <br/> |会議出席依頼の作成後の処理方法について説明します。 この属性は、予定表アイテムに必要です。  <br/> |
   
#### <a name="messagedisposition-attribute"></a>MessageDisposition 属性

|値|説明|
|:-----|:-----|
|SaveOnly  <br/> |メッセージ アイテムは [、SavedItemFolderId](saveditemfolderid.md) 要素で指定されたフォルダーに保存されます。 メッセージは、後で [SendItem 操作を使用して送信できます](senditem-operation.md)。 応答でアイテム識別子が返されます。 メッセージ アイテム以外のアイテムの種類に対して、アイテム識別子は返されません。 これには、応答オブジェクトも含まれます。  <br/> |
|SendOnly  <br/> |アイテムは送信されますが、コピーは送信済みアイテム フォルダーに保存されません。 アイテム識別子は応答では返されません。<br/><br/>**メモ**: **このオプションでは** 移動先フォルダーを指定できないので、SendOnly オプションを使用する場合、CreateItem は代理アクセスをサポートできません。 回避策は、アイテムを作成し、アイテム識別子を取得し、SendItem 操作を使用してアイテムを送信します。           |
|SendAndSaveCopy  <br/> |アイテムが送信され [、SavedItemFolderId](saveditemfolderid.md) 要素によって識別されるフォルダーにコピーが保存されます。 アイテム識別子は応答では返されません。<br/><br/>**メモ**: 会議出席依頼は [、SavedItemFolderId](saveditemfolderid.md) プロパティによって識別されるフォルダーには保存されません。 予定表の場合は **、SavedItemFolderId** プロパティで予定表アイテムの保存場所のみを指定できます。 会議出席依頼アイテムの保存場所を制御することはできません。 関連付けられた予定表アイテムだけがコピーされ **、SavedItemFolderId** プロパティによって識別されるフォルダーに保存されます。           |
   
#### <a name="sendmeetinginvitations-attribute"></a>SendMeetingInvitations 属性

|値|説明|
|:-----|:-----|
|SendToNone  <br/> |アイテムが会議出席依頼の場合、予定表アイテムとして保存されますが、送信されません。  <br/> |
|SendOnlyToAll  <br/> |会議出席依頼は、すべての出席者に送信されますが、[送信済みアイテム] フォルダーには保存されません。  <br/> |
|SendToAllAndSaveCopy  <br/> |会議出席依頼は、すべての出席者に送信され、コピーは [SavedItemFolderId](saveditemfolderid.md) 要素によって識別されるフォルダーに保存されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|要素|説明|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |新しいアイテムを作成できるターゲット フォルダーを識別します。 **MessageDisposition 属性が** SendOnly に設定されている場合は、作成されたメッセージだけが送信されます。 [メッセージは、SavedItemFolderId](saveditemfolderid.md)要素によって識別されるフォルダーに格納されません。  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |[SavedItemFolderId](saveditemfolderid.md)要素によって識別されるフォルダーに作成するアイテムの配列を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [CreateItemResponse](createitemresponse.md)  
- [CreateItem 操作](createitem-operation.md)
- [電子メール メッセージの作成](https://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [連絡先の作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [タスクの作成](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [予定の作成](https://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

