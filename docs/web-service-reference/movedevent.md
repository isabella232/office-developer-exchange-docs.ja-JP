---
title: MovedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MovedEvent
api_type:
- schema
ms.assetid: 572f8b40-dfa8-47bc-b0c1-e1a7138506fd
description: MovedEvent 要素は、ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。
ms.openlocfilehash: 4e0795fc3f335139e22fb51a4cf215a870ec62c6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518135"
---
# <a name="movedevent"></a>MovedEvent

**MovedEvent 要素** は、ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。 
  
```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldItemId/>
   <OldParentFolderId/>
</MovedEvent>
```

```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</MovedEvent>
```


**MovedCopiedEventType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |メールボックス イベント テーブルのイベント ブックマークを表します。  <br/> |
|[TimeStamp](timestamp.md) <br/> |移動アイテム/フォルダー メールボックス イベントのタイムスタンプを表します。  <br/> |
|[FolderId](folderid.md) <br/> |移動したフォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |移動したアイテムの識別子を表します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |移動したアイテムまたはフォルダーを含むフォルダーの識別子を表します。  <br/> |
|[OldFolderId](oldfolderid.md) <br/> |移動またはコピーする前の元のフォルダーのフォルダー識別子を格納します。  <br/> |
|[OldItemId](olditemid.md) <br/> |移動前の元のアイテムの一意の識別子を格納します。  <br/> |
|[OldParentFolderId](oldparentfolderid.md) <br/> |移動されたアイテムまたはフォルダーの元の親フォルダーの識別子を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションと、前回の通知以降に発生したイベントに関する情報が格納されます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [サブスクライブ操作](subscribe-operation.md) 
- [GetEvents 操作](getevents-operation.md) 
- [Unsubscribe 操作](unsubscribe-operation.md)

