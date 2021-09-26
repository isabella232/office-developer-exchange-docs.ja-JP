---
title: And
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- And
api_type:
- schema
ms.assetid: 790246c2-37ad-49a8-91b9-6186d743b011
description: And 要素は、2 つ以上の検索式の間でブール型 AND 演算を実行できる検索式を表します。 And 要素に含まれるすべての検索式が true の場合、AND 操作の結果は true になります。
ms.openlocfilehash: b6cf8ffbb19ea3aff917493e6ae4e324025c6ac9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541533"
---
# <a name="and"></a>And

**And 要素** は、2 つ以上の検索式の間で **ブール型 AND** 演算を実行できる検索式を表します。 **And** 要素に含まれるすべての検索式が true の場合 **、AND** 操作の結果は true **です**。
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 **AndType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | 制限内の式の基本クラスを表します。 And 操作には 2 つ以上の検索式が必要です。<br/><br/>  **SearchExpression** 要素では、次のいずれかの要素を置換する必要があります。<ul><li> [Exists](exists.md)</li><li>[Excludes](excludes.md)</li><li>[IsEqualTo](isequalto.md)</li><li>[IsNotEqualTo](isnotequalto.md)</li><li>[IsGreaterThan](isgreaterthan.md)</li><li>[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</li><li>[IsLessThan](islessthan.md)</li><li>[IsLessThanOrEqualTo](islessthanorequalto.md)</li><li>[Contains](contains.md)</li><li>[Not](not.md)</li><li>**And**</li><li>[Or](or.md) </li></ul> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |FindItem/FindFolder および検索フォルダー操作でアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれる検索式のブール値をネゲートする検索式を表します。  <br/> |
|**And** <br/> |2 つ以上の検索式の間で **ブール型 AND** 演算を実行できる検索式を表します。 **And** 要素に含まれるすべての検索式が true の場合 **、AND** 操作の結果は true **です**。  <br/> |
|[Or](or.md) <br/> |含まれる検索式に対して論理 **OR** 操作を実行する検索式を表します。 **または** 、子が **true** を返す場合は true を **返します**。 **または、2** つ以上の子が必要です。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

