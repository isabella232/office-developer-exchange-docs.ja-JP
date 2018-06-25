---
title: OldItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldItemId
api_type:
- schema
ms.assetid: fb57deee-9cc3-4730-9805-ff34f39e3ab7
description: OldItemId 要素には、コピーまたは移動された項目の一意の識別子が含まれています。
ms.openlocfilehash: ced7fc6891e0d1fde42a8cb9cad4f4e55493b5d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832648"
---
# <a name="olditemid"></a>OldItemId

**OldItemId**要素には、コピーまたは移動された項目の一意の識別子が含まれています。 
  
```xml
<OldItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |Exchange ストア内の項目を識別する文字列が含まれています。 この属性は、必要があります。  <br/> |
|**変更キー** <br/> |Id 属性によって識別される項目のバージョンを識別する文字列が含まれています。 この属性は、省略可能です。 アイテムの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーのコピー先のイベントを表します。  <br/> |
|[MovedEvent](movedevent.md) <br/> |アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。  <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
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

