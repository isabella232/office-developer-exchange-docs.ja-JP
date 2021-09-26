---
title: UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 34643d58-2743-45b0-a08d-bff6dc1da61d
description: UpdateItem 要素は、メールボックス内のアイテムを更新する要求を定義します。
ms.openlocfilehash: 544ccfb8c42b2a4d4f69ae04d383233203c235b8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542791"
---
# <a name="updateitem"></a>UpdateItem

**UpdateItem 要素** は、メールボックス内のアイテムを更新する要求を定義します。 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 **UpdateItemType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ConflictResolution** <br/> |更新中に試す競合解決の種類を識別します。 既定値は AutoResolve です。  <br/> |
|**MessageDisposition** <br/> |更新後のアイテムの処理方法について説明します。 **MessageDisposition** 属性は、会議のキャンセル、会議出席依頼、会議出席依頼などの会議メッセージを含むメッセージ アイテムに必要です。  <br/> |
|**SendMeetingInvitationsOrCancellations** <br/> |予定表アイテムの更新後に会議の更新プログラムがどのように通信されるのかについて説明します。 この属性は、予定表アイテムと予定表アイテムの出現に必要です。  <br/> |
|**SuppressReadReceipts** <br/> |更新されたアイテムの読み取りレシートを非表示にするかどうかを示します。 テキスト値が **true の場合** は、読み取りレシートを省略する必要があります。 false の **値は** 、読み取りレシートが送信者に送信されます。 この属性は省略可能です。  <br/> この属性は、2013 SP1 Exchange Server導入されました。  <br/> |
   
#### <a name="conflictresolution-attribute"></a>ConflictResolution 属性

|**値**|**説明**|
|:-----|:-----|
|NeverOverwrite  <br/> |競合がある場合、更新操作は失敗し、エラーが返されます。  <br/> |
|AutoResolve  <br/> |更新操作では、競合が自動的に解決されます。  <br/> |
|AlwaysOverwrite  <br/> |競合がある場合、更新操作によって情報が上書きされます。  <br/> |
   
#### <a name="messagedisposition-attribute"></a>MessageDisposition 属性

|**値**|**説明**|
|:-----|:-----|
|SaveOnly  <br/> |アイテムが更新され、現在のフォルダーに保存されます。  <br/> |
|SendOnly  <br/> |アイテムは更新され、送信されますが、コピーは保存されません。  <br/> |
|SendAndSaveCopy  <br/> |アイテムが更新され [、SavedItemFolderId](saveditemfolderid.md) 要素によって識別されるフォルダーにコピーが保存されます。  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a>SendMeetingInvitationsOrCancellations 属性

|**値**|**説明**|
|:-----|:-----|
|SendToNone  <br/> |予定表アイテムは更新されますが、更新は出席者に送信されません。  <br/> |
|SendOnlyToAll  <br/> |予定表アイテムが更新され、会議の更新がすべての出席者に送信されますが、[送信済みアイテム] フォルダーには保存されません。  <br/> |
|SendOnlyToChanged  <br/> |予定表アイテムが更新され、会議の更新は、会議の変更の影響を受ける出席者にのみ送信されます。  <br/> |
|SendToAllAndSaveCopy  <br/> |予定表アイテムが更新され、会議の更新がすべての出席者に送信され、コピーが [送信済みアイテム] フォルダーに保存されます。  <br/> |
|SendToChangedAndSaveCopy  <br/> |予定表アイテムが更新され、会議の変更の影響を受けるすべての出席者に会議の更新プログラムが送信され、コピーが [送信済みアイテム] フォルダーに保存されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |アイテムを更新、送信、および作成する操作のターゲット フォルダーを、Exchangeします。  <br/> |
|[ItemChanges](itemchanges.md) <br/> |アイテムとアイテムに適用する更新プログラムを識別する [ItemChange](itemchange.md) 要素の配列を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[UpdateItem 操作](updateitem-operation.md)

