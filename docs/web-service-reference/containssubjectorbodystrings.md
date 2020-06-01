---
title: ContainsSubjectOrBodyStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSubjectOrBodyStrings
api_type:
- schema
ms.assetid: 22aebf31-d9f4-4e03-bbff-c675409518d1
description: ContainsSubjectOrBodyStrings 要素は、条件または例外を適用するために、受信メッセージの本文または件名に表示する必要がある文字列を示します。
ms.openlocfilehash: 6f9c7862912632e7e86a0b704e760c7fd0f5f14c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466823"
---
# <a name="containssubjectorbodystrings"></a>ContainsSubjectOrBodyStrings

**ContainsSubjectOrBodyStrings**要素は、条件または例外を適用するために、受信メッセージの本文または件名に表示する必要がある文字列を示します。 
  
```XML
<ContainsSubjectOrBodyStrings>
    <String/>
</ContainsSubjectOrBodyStrings>
```

 **ArrayOfStringsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[String](string.md) <br/> |条件または例外を適用するために、受信メッセージの本文または件名のどちらかに表示される文字列を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[条件](conditions.md) <br/> |ルールのルールの処理を開始するときに実行される条件を表します。  <br/> |
|[例外](exceptions.md) <br/> |受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

