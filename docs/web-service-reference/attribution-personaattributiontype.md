---
title: Attribution (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: Attributes 要素は、PersonaType 要素の属性の配列内のインスタンスを指定します。
ms.openlocfilehash: eb2fe66042b6c7f52732be20195f0f4b94ab867c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524379"
---
# <a name="attribution-personaattributiontype"></a>Attribution (PersonaAttributionType)

**Attributes 要素** は **、PersonaType** 要素の属性の配列内のインスタンスを指定します。 
  
```XML
<Attribution>
    <Id></Id>
    <SourceId></SourceId>
    <DisplayName></DisplayName>
    <IsWritable></IsWritable>
    <IsQuickContact></IsQuickContact>
    <IsHidden></IsHidden>
    <FolderId></FolderId>
</Attribution>
```

 **PersonaAttributionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ID (String)](id-string.md) <br/> |ペルサのアプリまたは属性を一意に識別する文字列を指定します。  <br/> |
|[SourceId](sourceid.md) <br/> |連絡先または Active Directory 受信者の識別子を指定します。  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |フォルダー、連絡先、配布リスト、委任ユーザー、またはルールの表示名を定義します。  <br/> |
|[IsWritable](iswritable.md) <br/> |基になる連絡先または Active Directory 受信者を書き込むかどうかを指定します。  <br/> |
|[IsQuickContact](isquickcontact.md) <br/> |基になる連絡先または Active Directory 受信者がクイック連絡先であるかどうかを示すブール値を指定します。  <br/> |
|[IsHidden](ishidden.md) <br/> |基になる連絡先または Active Directory 受信者を非表示にするか、ペルサの一部として表示するかどうかを示すブール値を含む。  <br/> |
|[FolderId](folderid.md) <br/> |フォルダーの識別子と変更キーを格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) <br/> |関連付けられたペルサに集約された 1 つ以上の連絡先またはアクティブ ディレクトリ (AD) 受信者の属性情報の配列を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

