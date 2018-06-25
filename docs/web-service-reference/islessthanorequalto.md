---
title: IsLessThanOrEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsLessThanOrEqualTo
api_type:
- schema
ms.assetid: b5d85eb2-5e15-4d01-ad49-6289e735ad8a
description: IsLessThanOrEqualTo 要素をプロパティに定数値または別のプロパティを比較し、最初のプロパティは、2 番目に等しいかそれより小さい場合は true を返す検索式を表します。
ms.openlocfilehash: 9aeb688ec68e13635ac3083119899bcd55045f7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832043"
---
# <a name="islessthanorequalto"></a>IsLessThanOrEqualTo

**IsLessThanOrEqualTo**要素は、最初のプロパティが、1 秒未満である場合、プロパティを定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。 
  
```xml
<IsLessThanOrEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsLessThanOrEqualTo>
```

 **IsLessThanOrEqualToType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々 のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |MAPI プロパティを識別します。  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |プロパティまたは別のプロパティを比較するときに使用する定数値のいずれかを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれている検索式のブール値を否定する検索式を表します。  <br/> |
|[And](and.md) <br/> |使用すると、2 つまたは複数の検索式間で論理 And 演算を実行する検索式を表します。 **すべての And に含まれている検索式に**該当**する場合は、And 演算の結果は**  <br/> |
|[Or](or.md) <br/> |含まれている検索式に対して論理 OR を実行する検索式を表します。 [または](or.md) **true**を返します true を返す任意の子の場合。 [または](or.md)2 つ以上の子が必要です。  <br/> |
   
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



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

