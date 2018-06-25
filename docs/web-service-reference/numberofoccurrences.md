---
title: NumberOfOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfOccurrences
api_type:
- schema
ms.assetid: 9ec86ceb-b271-4718-97ca-b6a532ea7223
description: NumberOfOccurrences 要素には、定期的なアイテムの出現回数が含まれています。
ms.openlocfilehash: c18a20f14395aead304bd0158ff64c70e51ec165
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832656"
---
# <a name="numberofoccurrences"></a>NumberOfOccurrences

**NumberOfOccurrences**要素には、定期的なアイテムの出現回数が含まれています。 
  
```xml
<NumberOfOccurrences/>
```

 **int**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[NumberedRecurrence](numberedrecurrence.md) <br/> |開始日と定期的なアイテムの出現回数を説明します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、定期的なアイテムの出現回数を表す整数です。 値は 1 ~ 999 の範囲の整数である必要があります。
  
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

