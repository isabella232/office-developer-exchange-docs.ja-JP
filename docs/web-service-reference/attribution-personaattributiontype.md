---
title: 属性 (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: 属性要素は、個人の Atype 要素の属性の配列のインスタンスを指定します。
ms.openlocfilehash: 05b0d41c116f2ed7b8dbb3ac44108bb879256b5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464176"
---
# <a name="attribution-personaattributiontype"></a>属性 (PersonaAttributionType)

属性**要素は、** **個人の atype**要素の属性の配列のインスタンスを指定します。 
  
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
|[ID (文字列)](id-string.md) <br/> |アプリを一意に識別する文字列を指定します。または、ペルソナの属性を指定します。  <br/> |
|[SourceId](sourceid.md) <br/> |連絡先または Active Directory 受信者の識別子を指定します。  <br/> |
|[DisplayName (文字列)](displayname-string.md) <br/> |フォルダー、連絡先、配布リスト、代理人のユーザー、またはルールの表示名を定義します。  <br/> |
|[IsWritable 可能](iswritable.md) <br/> |基になる連絡先または Active Directory 受信者に書き込むことができるかどうかを指定します。  <br/> |
|[IsQuickContact](isquickcontact.md) <br/> |基になる連絡先または Active Directory 受信者がクイック連絡先であるかどうかを示すブール値を指定します。  <br/> |
|[IsHidden](ishidden.md) <br/> |基になる連絡先または Active Directory 受信者を表示するか、ペルソナの一部として表示するかを示すブール値を格納します。  <br/> |
|[FolderId](folderid.md) <br/> |フォルダーの識別子と変更キーが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) <br/> |関連付けられたペルソナに集約された1つ以上の連絡先または active directory (AD) 受信者の属性情報の配列を指定します。  <br/> |
   
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

