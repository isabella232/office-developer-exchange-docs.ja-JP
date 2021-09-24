---
title: SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SendItem
api_type:
- schema
ms.assetid: a966da19-b05a-4504-ac98-91acc1667b9a
description: SendItem 要素は、アイテムをストアに送信する要求のルートExchangeです。
ms.openlocfilehash: 2d1613451e7f876f0b612a3249570412e40b4764
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521621"
---
# <a name="senditem"></a>SendItem

**SendItem 要素** は、メッセージ ストア内のアイテムを送信する要求のルートExchangeです。 
  
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
|**SaveItemToFolder** <br/> |送信済みアイテムのコピーを保存するかどうかを指定します。 保存アクションは **、SaveItemToFolder** の値と [、SaveItemFolderId](saveditemfolderid.md) 要素が要求に存在するかどうかによって異なります。 この要素は必須です。  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a>SaveItemToFolder 属性

|**値**|**説明**|
|:-----|:-----|
|**true** <br/> |[SavedItemFolderId](saveditemfolderid.md)要素が存在しない場合、アイテムは [送信済みアイテム] フォルダーに保存されます。 [SavedItemFolderId 要素が存在](saveditemfolderid.md)する場合、そのアイテムは[SavedItemFolderId](saveditemfolderid.md)要素で指定されたフォルダーに保存されます。  <br/> |
|**false** <br/> |[SavedItemFolderId](saveditemfolderid.md)要素が存在しない場合、アイテムは保存されません。 [SavedItemFolderId](saveditemfolderid.md)要素が存在する場合 **、ErrorInvalidSendItemSaveSettings** 値を含む [ResponseCode](responsecode.md)要素でエラー応答が返されます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用されるアイテム、オカレンス アイテム、および定期的なマスター アイテムの一意の ID をExchangeします。  <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> |アイテムを更新、送信、および作成する操作のターゲット フォルダーを、Exchangeします。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

送信済みアイテム フォルダー内のアイテムが送信された場合、送信済みアイテムは削除され、そのコピーが [送信済みアイテム] フォルダーに格納されます。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[SendItem 操作](senditem-operation.md)

