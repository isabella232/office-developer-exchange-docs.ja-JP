---
title: SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: a966da19-b05a-4504-ac98-91acc1667b9a
description: SendItem 要素は、Exchange ストア内のアイテムを送信する要求のルート要素です。
ms.openlocfilehash: c5ce52ee4643219aa31ae59e8b7d40d7a904c8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833340"
---
# <a name="senditem"></a>SendItem

**SendItem**要素は、Exchange ストア内のアイテムを送信する要求のルート要素です。 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 **SendItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**SaveItemToFolder** <br/> |送信済みアイテムのコピーを保存するかどうかを識別します。 保存アクションは、 **SaveItemToFolder**と[SavedItemFolderId](saveditemfolderid.md)要素が要求内に存在するかどうかの値によって異なります。 この要素は必須です。  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a>SaveItemToFolder 属性

|**値**|**説明**|
|:-----|:-----|
|**true** <br/> |[SavedItemFolderId](saveditemfolderid.md)要素が存在しない場合は、送信済みアイテム フォルダーにアイテムを保存します。 [SavedItemFolderId](saveditemfolderid.md)要素が存在する場合、 [SavedItemFolderId](saveditemfolderid.md)要素で指定されているフォルダーにアイテムを保存します。  <br/> |
|**false** <br/> |[SavedItemFolderId](saveditemfolderid.md)要素が存在しない場合は、アイテムは保存されません。 [SavedItemFolderId](saveditemfolderid.md)要素が存在する場合、 **ErrorInvalidSendItemSaveSettings**値を格納する[ResponseCode](responsecode.md)要素を使用して、エラー応答が返されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Itemid](itemids.md) <br/> |アイテム、出現アイテム、および削除、送信、取得、移動、または Exchange ストア内のアイテムのコピーに使用される、マスターの定期的なアイテムの一意の id が含まれています。  <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> |更新、送信、および Exchange ストア内の項目を作成する操作のターゲット フォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

送信済みアイテム フォルダー内のアイテムが送信された場合、送信済みアイテムを削除しのコピーが送信済みアイテム フォルダーに配置します。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [SendItem 操作](senditem-operation.md)

