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
description: CreateItem 要素は、Exchange ストア内のアイテムを作成する要求を定義します。
ms.openlocfilehash: bb5cddd5ea4fa1b73c424275a0b0219ce3e189e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759840"
---
# <a name="createitem"></a>CreateItem

**CreateItem**要素は、Exchange ストア内のアイテムを作成する要求を定義します。 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

 **CreateItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MessageDisposition** <br/> |作成後のアイテムの処理方法について説明します。 属性は、電子メール メッセージに必要です。 この属性は、電子メール メッセージに該当する場合のみです。  <br/> |
|**SendMeetingInvitations** <br/> |作成後に会議出席依頼を処理する方法について説明します。 この属性は、予定表アイテムの必要があります。  <br/> |
   
#### <a name="messagedisposition-attribute"></a>MessageDisposition 属性

|**値**|**説明**|
|:-----|:-----|
|SaveOnly  <br/> |メッセージ アイテムは、 [SavedItemFolderId](saveditemfolderid.md)要素で指定されているフォルダーに保存されます。 [SendItem 操作](senditem-operation.md)を使用してメッセージを後で送信することができます。 アイテム識別子は、応答で返されます。 メッセージ アイテム以外の項目の種類の項目の識別子は返されません。 これには、応答オブジェクトが含まれます。  <br/> |
|SendOnly  <br/> |アイテムを送信しますが、送信済みアイテム フォルダーにコピーは保存されません。 アイテム識別子は、応答で返されません。  <br/> > [!NOTE]> **Createitem メソッド**は、このオプションを使用してインストール先のフォルダーを指定することはできませんので、SendOnly オプションを使用する場合、代理人アクセスをサポートされていません。 回避するに項目を作成し、項目の識別子を取得する、SendItem 操作を使用して、アイテムを送信するには。           |
|SendAndSaveCopy  <br/> |アイテムが送信され、 [SavedItemFolderId](saveditemfolderid.md)要素で指定されているフォルダーにコピーが保存されます。 アイテム識別子は、応答で返されません。  <br/> > [!NOTE]> 会議出席依頼は、 [SavedItemFolderId](saveditemfolderid.md)プロパティで指定されたフォルダーに保存されません。 予定表の作成、保存だけの**SavedItemFolderId**プロパティによって予定表アイテムの場所を指定することができます。 会議出席依頼アイテムの保存場所を制御することはできません。 関連付けられている予定表アイテムのみがコピーされ、 **SavedItemFolderId**プロパティで指定されたフォルダーに保存されます。           |
   
#### <a name="sendmeetinginvitations-attribute"></a>SendMeetingInvitations 属性

|**値**|**説明**|
|:-----|:-----|
|SendToNone  <br/> |アイテムが会議出席依頼の場合は、これは予定表のアイテムとして保存しますが、送信されません。  <br/> |
|SendOnlyToAll  <br/> |会議出席依頼は、すべての出席者に送信されますが、送信済みアイテム フォルダーには保存されません。  <br/> |
|SendToAllAndSaveCopy  <br/> |すべての出席者に会議出席依頼が送信され、 [SavedItemFolderId](saveditemfolderid.md)要素で指定されているフォルダーにコピーが保存されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |新しいアイテムを作成することができますターゲット フォルダーを識別します。 **MessageDisposition**属性は、SendOnly に設定されている場合は、作成したメッセージのみ送信されます。 [SavedItemFolderId](saveditemfolderid.md)要素で指定されたフォルダーにメッセージは送信されません。  <br/> |
|[アイテム (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |[SavedItemFolderId](saveditemfolderid.md)要素で指定されたフォルダーに作成する項目の配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateItemResponse](createitemresponse.md)
  

  [CreateItem 操作](createitem-operation.md)
  
 **CreateItemType**


[電子メール メッセージの作成](http://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx)
  
[連絡先 (Exchange Web サービス) を作成します。](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[タスクを作成します。](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[予定の作成](http://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

