---
title: UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 34643d58-2743-45b0-a08d-bff6dc1da61d
description: UpdateItem 要素では、メールボックス内のアイテムを更新する要求を定義します。
ms.openlocfilehash: 7b9b5f1dcffb95eb127572cb91f92d961c05a77e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/21/2018
ms.locfileid: "19839869"
---
# <a name="updateitem"></a>UpdateItem

**UpdateItem**要素では、メールボックス内のアイテムを更新する要求を定義します。 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 **UpdateItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ConflictResolution** <br/> |更新中に競合の解決の種類を識別します。 既定値は、自動解決します。  <br/> |
|**MessageDisposition** <br/> |更新後のアイテムの処理方法について説明します。 **MessageDisposition**属性は、メッセージ アイテム、会議の取り消し、会議出席依頼、会議出席依頼など、会議のメッセージを含む必要があります。  <br/> |
|**SendMeetingInvitationsOrCancellations** <br/> |予定表アイテムが更新された後に会議の更新を通知する方法について説明します。 この属性は、予定表アイテム、予定表アイテムの出現する必要があります。  <br/> |
|**SuppressReadReceipts** <br/> |更新されたアイテムの開封確認メッセージを抑制するかどうかを示します。 **True**の場合、テキスト値では、読み取り確認メッセージを抑制するかを示します。 **False**の値は、送信者に開封確認が送信されることを示します。 この属性は、省略可能です。  <br/> この属性は、Exchange Server 2013 SP1 で導入されました。  <br/> |
   
#### <a name="conflictresolution-attribute"></a>ConflictResolution 属性

|**値**|**説明**|
|:-----|:-----|
|NeverOverwrite  <br/> |競合がある場合は、更新操作は失敗し、エラーが返されます。  <br/> |
|自動解決  <br/> |更新操作は、自動的にすべての競合を解決します。  <br/> |
|AlwaysOverwrite  <br/> |競合がある場合は、更新操作には情報が上書きされます。  <br/> |
   
#### <a name="messagedisposition-attribute"></a>MessageDisposition 属性

|**値**|**説明**|
|:-----|:-----|
|SaveOnly  <br/> |アイテムが更新され、現在のフォルダーに保存します。  <br/> |
|SendOnly  <br/> |アイテムが更新され、送信されたが、コピーは保存されません。  <br/> |
|SendAndSaveCopy  <br/> |アイテムを更新し、 [SavedItemFolderId](saveditemfolderid.md)要素で指定されたフォルダーにコピーを保存します。  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a>SendMeetingInvitationsOrCancellations 属性

|**値**|**説明**|
|:-----|:-----|
|SendToNone  <br/> |予定表アイテムが更新されますが、更新が出席者に送信されません。  <br/> |
|SendOnlyToAll  <br/> |予定表アイテムが更新され、会議の更新は、すべての出席者に送信されますが、送信済みアイテム フォルダーには保存されません。  <br/> |
|SendOnlyToChanged  <br/> |予定表アイテムが更新され、会議の更新は、会議の変更の影響を受けるための出席者にのみ送信します。  <br/> |
|SendToAllAndSaveCopy  <br/> |予定表アイテムが更新され、すべての出席者に会議の更新が送信されるコピーが [送信済みアイテム フォルダーに保存されます。  <br/> |
|SendToChangedAndSaveCopy  <br/> |予定表アイテムが更新され、会議の変更の影響を受けるすべての出席者に会議の更新が送信されるコピーが [送信済みアイテム フォルダーに保存されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |更新、送信、および Exchange ストア内の項目を作成する操作のターゲット フォルダーを識別します。  <br/> |
|[ItemChanges](itemchanges.md) <br/> |アイテムと、アイテムに適用する更新プログラムを識別する[ItemChange](itemchange.md)要素の配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [UpdateItem 操作](updateitem-operation.md)

