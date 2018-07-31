---
title: FieldURIOrConstant
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldURIOrConstant
api_type:
- schema
ms.assetid: 89d7a87e-7c93-49b8-83ec-8798e08c1052
description: FieldURIOrConstant 要素は、プロパティ、または別のプロパティを比較するときに使用する定数値を表します。
ms.openlocfilehash: a24c2fa044e03d0ac6f900625e325600903df8d0
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354226"
---
# <a name="fielduriorconstant"></a>FieldURIOrConstant

**FieldURIOrConstant**要素は、プロパティ、または別のプロパティを比較するときに使用する定数値を表します。 
  
```xml
<FieldURIOrConstant>
   <Constant/>
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
    <IndexedFieldURI/> 
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
   <FieldURI/>
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
   <ExtendedFieldURI/> 
</FieldURIOrConstant>
```

**FieldURIOrConstantType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[定数](constant.md) <br/> |制限における定数値を識別します。  <br/> |
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々 のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |MAPI プロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[IsEqualTo](isequalto.md) <br/> |プロパティを定数値または別のプロパティを比較し、両者が等しい場合に true に評価する検索式を表します。  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |定数値を持つプロパティ、または別のプロパティを比較し、最初のプロパティ値が大きい場合に true を返す検索式を表します。  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |プロパティに定数値または別のプロパティを比較し、true を指定すると、最初のプロパティは、以上の 2 番目の値またはプロパティに値を返す検索式を表します。  <br/> |
|[IsLessThan](islessthan.md) <br/> |定数値を持つプロパティ、または別のプロパティを比較し、最初のプロパティは、2 番目の値やプロパティよりも小さい場合は true を返す検索式を表します。  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |定数値を持つプロパティ、または別のプロパティを比較し、最初のプロパティは、2 番目の値またはプロパティに等しいかそれより小さい場合は true を返す検索式を表します。  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |定数値を持つプロパティ、または別のプロパティを比較し、値が同じではない場合は true を返す検索式を表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

次の XML の例では、定数と URI のフィールドの両方で使用する FieldURIOrConstant 要素を示します。
  
```xml
<Restriction>
  <Or xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
    <IsEqualTo>
      <FieldURI FieldURI="item:DateTimeCreated"/>
      <FieldURIOrConstant>
        <FieldURI FieldURI="item:DateTimeReceived"/>
      </FieldURIOrConstant>
    </IsEqualTo>
    <IsEqualTo>
      <FieldURI FieldURI="item:Subject"/>
      <FieldURIOrConstant>
        <Constant Value="Here is a test message"/>
      </FieldURIOrConstant>
    </IsEqualTo>
  </Or>
</Restriction>
```

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

