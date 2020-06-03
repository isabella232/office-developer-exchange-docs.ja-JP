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
description: SendItem 要素は、Exchange ストア内のアイテムを送信するための要求のルート要素です。
ms.openlocfilehash: 28f0d484dd079146c998cb7317bd2d80c6739e19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530566"
---
# <a name="senditem"></a>SendItem

**SendItem**要素は、Exchange ストア内のアイテムを送信するための要求のルート要素です。 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 **SendItemType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**SaveItemToFolder** <br/> |送信されたアイテムのコピーを保存するかどうかを指定します。 Save アクションは、 **Saveitemtofolder**の値と、要求に[SavedItemFolderId](saveditemfolderid.md)要素が存在するかどうかによって異なります。 この要素は必須です。  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a>SaveItemToFolder 属性

|**値**|**説明**|
|:-----|:-----|
|**true** <br/> |[SavedItemFolderId](saveditemfolderid.md)要素が存在しない場合、アイテムは [送信済みアイテム] フォルダーに保存されます。 [SavedItemFolderId](saveditemfolderid.md)要素が存在する場合は、 [SavedItemFolderId](saveditemfolderid.md)要素によって指定されたフォルダーにアイテムが保存されます。  <br/> |
|**false** <br/> |[SavedItemFolderId](saveditemfolderid.md)要素が存在しない場合、アイテムは保存されません。 [SavedItemFolderId](saveditemfolderid.md)要素が存在する場合は、エラー応答が返されます。この値は、 **Errorinvalidsenditemsavesettings**値を[含む、応答](responsecode.md)します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用されるアイテム、オカレンスアイテム、定期的なマスターアイテムの一意の id が含まれています。  <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Exchange ストア内のアイテムを更新、送信、および作成する操作のターゲットフォルダーを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

送信済みアイテムフォルダー内のアイテムが送信されると、送信されたアイテムは削除され、そのコピーが [送信済みアイテム] フォルダーに配置されます。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[SendItem 操作](senditem-operation.md)

