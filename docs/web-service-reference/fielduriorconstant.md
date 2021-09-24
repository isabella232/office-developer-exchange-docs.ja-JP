---
title: FieldURIOrConstant
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FieldURIOrConstant
api_type:
- schema
ms.assetid: 89d7a87e-7c93-49b8-83ec-8798e08c1052
description: FieldURIOrConstant 要素は、別のプロパティと比較するときに使用するプロパティまたは定数値を表します。
ms.openlocfilehash: bc7edb4542c68e02e9661ff0a4c7066362a04081
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535242"
---
# <a name="fielduriorconstant"></a>FieldURIOrConstant

**FieldURIOrConstant** 要素は、別のプロパティと比較するときに使用するプロパティまたは定数値を表します。 
  
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

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[定数](constant.md) <br/> |制限内の定数値を識別します。  <br/> |
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |MAPI プロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[IsEqualTo](isequalto.md) <br/> |プロパティと定数値または別のプロパティを比較し、等しい場合は true と評価される検索式を表します。  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |プロパティを定数値または別のプロパティと比較する検索式を表し、最初のプロパティが大きい場合は true を返します。  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが 2 番目の値またはプロパティ以上の場合は true を返す検索式を表します。  <br/> |
|[IsLessThan](islessthan.md) <br/> |プロパティを定数値または別のプロパティと比較する検索式を表し、最初のプロパティが 2 番目の値またはプロパティより小さい場合は true を返します。  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが 2 番目の値またはプロパティ以下の場合は true を返す検索式を表します。  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |定数値または別のプロパティとプロパティを比較する検索式を表し、値が同じではない場合は true を返します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

次の XML 例は、定数 URI とフィールド URI の両方で使用される FieldURIOrConstant 要素を示しています。
  
```xml
<Restriction>
  <Or xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

