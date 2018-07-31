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
description: MovedEvent 要素は、アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。
ms.openlocfilehash: 07f9c02ea194187a9fdfb1e27b19eb311392f51f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353260"
---
# <a name="movedevent"></a>MovedEvent

**MovedEvent**要素は、アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。 
  
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |メールボックス イベント テーブル内のイベント ブックマークを表します。  <br/> |
|[TimeStamp](timestamp.md) <br/> |移動アイテムまたはフォルダーのメールボックス イベントのタイムスタンプを表します。  <br/> |
|[FolderId](folderid.md) <br/> |移動したフォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |移動された項目の識別子を表します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |移動したアイテムまたはフォルダーを含むフォルダーの識別子を表します。  <br/> |
|[OldFolderId](oldfolderid.md) <br/> |移動またはコピーする前に元のフォルダーのフォルダーの識別子が含まれています。  <br/> |
|[OldItemId](olditemid.md) <br/> |移動する前に元のアイテムの一意の識別子が含まれています。  <br/> |
|[OldParentFolderId](oldparentfolderid.md) <br/> |アイテムまたはフォルダーの移動元の親フォルダーの識別子が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。  <br/> |
   
## <a name="remarks"></a>注釈

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [サブスクライブ操作](subscribe-operation.md) 
- [GetEvents 操作](getevents-operation.md) 
- [Unsubscribe 操作](unsubscribe-operation.md)

