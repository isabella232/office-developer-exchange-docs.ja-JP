---
title: MovedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MovedEvent
api_type:
- schema
ms.assetid: 572f8b40-dfa8-47bc-b0c1-e1a7138506fd
description: MovedEvent 要素は、ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。
ms.openlocfilehash: 1f8fb57dba7edb769fe0dd658d89c032dccf8c5f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530409"
---
# <a name="movedevent"></a>MovedEvent

**Movedevent**要素は、ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。 
  
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
|[Watermark](watermark.md) <br/> |メールボックスイベントテーブルのイベントブックマークを表します。  <br/> |
|[示](timestamp.md) <br/> |移動アイテム/フォルダーメールボックスイベントのタイムスタンプを表します。  <br/> |
|[FolderId](folderid.md) <br/> |移動されたフォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |移動されたアイテムの識別子を表します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |移動したアイテムまたはフォルダーを含むフォルダーの識別子を表します。  <br/> |
|[OldFolderId](oldfolderid.md) <br/> |移動またはコピーされる前の元のフォルダーのフォルダー識別子を含みます。  <br/> |
|[OldItemId](olditemid.md) <br/> |移動される前の元のアイテムの一意識別子を含みます。  <br/> |
|[OldParentFolderId](oldparentfolderid.md) <br/> |移動されたアイテムまたはフォルダーの元の親フォルダーの識別子が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [サブスクライブ操作](subscribe-operation.md) 
- [GetEvents 操作](getevents-operation.md) 
- [Unsubscribe 操作](unsubscribe-operation.md)

