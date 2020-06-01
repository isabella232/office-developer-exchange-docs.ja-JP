---
title: ユーザー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65312428-548c-4fe9-971a-d0dab3be5ddf
description: People 要素は、FindPeople 要求の結果として返されるペルソナデータの配列を指定します。
ms.openlocfilehash: b3920ca5cdf1d219c5fe119caeaaaf4965c39794
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467187"
---
# <a name="people"></a>ユーザー

**People**要素は、 **findpeople**要求の結果として返されるペルソナデータの配列を指定します。 
  
```XML
<People>
   <Persona/>
</People>
```

**ArrayOfPeopleType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ユーザー](persona.md)
  
### <a name="parent-elements"></a>親要素

[FindPeopleResponse](findpeopleresponse.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> ||
   

