---
title: 出現
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: d292b99c-b896-40b7-be5d-2cb314c9481f
description: 見つかった要素では、定期的な予定表アイテムの 1 つの変更されたアイテムを表します。
ms.openlocfilehash: 5a40faa9b885a235d30e7f41830d1eefe2ed23c3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832653"
---
# <a name="occurrence"></a>出現

**見つかった**要素では、定期的な予定表アイテムの 1 つの変更されたアイテムを表します。 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

**OccurrenceInfoType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |定期的な予定表アイテムに変更されたアイテムの一意の識別子と変更キーが含まれています。  <br/> |
|[Start](start.md) <br/> |定期的な予定表アイテムに変更されたアイテムの開始時刻を表します。  <br/> |
|[終わり](end-ex15websvcsotherref.md) <br/> |定期的な予定表アイテムに変更されたアイテムの終了時刻を表します。  <br/> |
|[OriginalStart](originalstart.md) <br/> |定期的な予定表アイテムに変更されたアイテムの元の開始時刻を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |定期的な予定のマスター アイテムとは異なるものに変更された定期的な予定表アイテム アイテムのコレクションが含まれています。  <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

