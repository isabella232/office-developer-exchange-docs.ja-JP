---
title: OldParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldParentFolderId
api_type:
- schema
ms.assetid: da1b8c88-c650-455d-b749-0cd160b012d8
description: OldParentFolderId 要素には、アイテムまたはフォルダーをコピーまたは移動の親フォルダーの識別子が含まれています。
ms.openlocfilehash: 1c4a51755c4194939dd797efa31cf5410b02bf85
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832644"
---
# <a name="oldparentfolderid"></a>OldParentFolderId

**OldParentFolderId**要素には、アイテムまたはフォルダーをコピーまたは移動の親フォルダーの識別子が含まれています。 
  
```xml
<OldParentFolderId Id="" ChangeKey=""/>
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |Exchange ストア内のフォルダーを識別する文字列が含まれています。 この属性は、必要があります。  <br/> |
|**変更キー** <br/> |Id 属性によって識別されるフォルダーのバージョンを識別する文字列が含まれています。 この属性は、省略可能です。 フォルダーの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーのコピー先のイベントを表します。  <br/> |
|[MovedEvent](movedevent.md) <br/> |アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

