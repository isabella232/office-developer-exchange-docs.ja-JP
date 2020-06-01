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
description: UpdateItem 要素は、メールボックス内のアイテムを更新する要求を定義します。
ms.openlocfilehash: 43821db58457ffce22be918a7ba6427f57230010
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466571"
---
# <a name="updateitem"></a>UpdateItem

**Updateitem**要素は、メールボックス内のアイテムを更新する要求を定義します。 
  
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
|**ConflictResolution** <br/> |更新中に試行する競合解決の種類を識別します。 既定値は自動解決です。  <br/> |
|**MessageDisposition** <br/> |アイテムが更新された後の処理方法について説明します。 **MessageDisposition**属性は、会議の取り消し、会議出席依頼、会議の返信などの会議メッセージを含む、メッセージアイテムに必要です。  <br/> |
|**SendMeetingInvitationsOrCancellations** <br/> |予定表アイテムが更新された後に、会議の更新が伝達される方法について説明します。 この属性は、予定表アイテムと予定表アイテムの出現に必要です。  <br/> |
|**SuppressReadReceipts** <br/> |更新されたアイテムの開封確認を抑制するかどうかを示します。 テキスト値が**true の場合**、開封確認を抑制する必要があることを示します。 値が**false**の場合、開封確認が送信者に送信されることを示します。 この属性は省略可能です。  <br/> この属性は、Exchange Server 2013 SP1 で導入されました。  <br/> |
   
#### <a name="conflictresolution-attribute"></a>ConflictResolution 属性

|**値**|**説明**|
|:-----|:-----|
|NeverOverwrite  <br/> |競合がある場合は、更新操作が失敗し、エラーが返されます。  <br/> |
|解決  <br/> |Update 操作は、競合を自動的に解決します。  <br/> |
|AlwaysOverwrite  <br/> |競合がある場合は、更新操作によって情報が上書きされます。  <br/> |
   
#### <a name="messagedisposition-attribute"></a>MessageDisposition 属性

|**値**|**説明**|
|:-----|:-----|
|SaveOnly  <br/> |アイテムが更新され、現在のフォルダーに戻されます。  <br/> |
|SendOnly  <br/> |アイテムは更新されて送信されますが、コピーは保存されません。  <br/> |
|SendAndSaveCopy  <br/> |アイテムが更新され、 [SavedItemFolderId](saveditemfolderid.md)要素によって識別されるフォルダーにコピーが保存されます。  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a>SendMeetingInvitationsOrCancellations 属性

|**値**|**説明**|
|:-----|:-----|
|SendToNone  <br/> |予定表アイテムは更新されますが、更新プログラムは出席者に送信されません。  <br/> |
|SendOnlyToAll  <br/> |予定表アイテムが更新され、会議の更新がすべての出席者に送信されますが、[送信済みアイテム] フォルダーには保存されません。  <br/> |
|SendOnlyToChanged  <br/> |予定表アイテムが更新され、会議の変更の影響を受ける出席者にのみ会議の更新が送信されます。  <br/> |
|SendToAllAndSaveCopy  <br/> |予定表アイテムが更新されると、会議の更新はすべての出席者に送信され、コピーは [送信済みアイテム] フォルダーに保存されます。  <br/> |
|SendToChangedAndSaveCopy  <br/> |予定表アイテムが更新されると、会議の変更の影響を受けるすべての出席者に会議の更新が送信され、[送信済みアイテム] フォルダーにコピーが保存されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Exchange ストア内のアイテムを更新、送信、および作成する操作のターゲットフォルダーを指定します。  <br/> |
|[ItemChanges](itemchanges.md) <br/> |アイテムとアイテムに適用する更新を識別する[Itemchange](itemchange.md)要素の配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目




  [UpdateItem 操作](updateitem-operation.md)

