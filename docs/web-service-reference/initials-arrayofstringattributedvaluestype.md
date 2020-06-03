---
title: イニシャル (ArrayOfStringAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 060c0cf1-c632-484c-87f5-f577017a7090
description: '[イニシャル] 要素は、イニシャル値の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。'
ms.openlocfilehash: 16133192fa1d9ef066e46a181f490248a8197e5b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458202"
---
# <a name="initials-arrayofstringattributedvaluestype"></a>イニシャル (ArrayOfStringAttributedValuesType)

[**イニシャル**] 要素は、イニシャル値の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。 
  
```XML
<Initials>
    <StringAttributedValue/>
</Initials>
```

 **ArrayOfStringAttributedValuesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[StringAttributedValue](stringattributedvalue.md) <br/> |Persona 要素に関連付けられている属性の配列のインスタンスを指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ユーザー](persona.md) <br/> |**Getpersona**要求によって返される一連のペルソナデータを指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

