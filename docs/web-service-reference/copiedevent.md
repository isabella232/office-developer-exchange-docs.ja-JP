---
title: CopiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopiedEvent
api_type:
- schema
ms.assetid: 82f2fcac-deaa-4ff8-801f-4fe28d8a19f5
description: CopiedEvent 要素は、アイテムまたはフォルダーがコピーされるイベントを表します。
ms.openlocfilehash: 928910ddbe0bf1e48549d1665ab373f7382366d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529246"
---
# <a name="copiedevent"></a>CopiedEvent

**Copiedevent**要素は、アイテムまたはフォルダーがコピーされるイベントを表します。 
  
```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
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
|[示](timestamp.md) <br/> |コピーアイテム/フォルダーメールボックスイベントのタイムスタンプを表します。  <br/> |
|[FolderId](folderid.md) <br/> |フォルダーの識別子を表します。  <br/> |
|[ItemId](itemid.md) <br/> |アイテムの識別子を表します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |コピーが格納されているフォルダーの識別子を表します。  <br/> |
|[OldFolderId](oldfolderid.md) <br/> |コピー前の元のフォルダーのフォルダー識別子を表します。  <br/> |
|[OldItemId](olditemid.md) <br/> |コピーされる前の元のアイテムの一意識別子を含みます。  <br/> |
|[OldParentFolderId](oldparentfolderid.md) <br/> |コピーされたアイテムまたはフォルダーの元の親フォルダーの識別子が含まれています。  <br/> |
   
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
- [プルサブスクリプションの使用](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [プッシュ通知のサンプル アプリケーション](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

