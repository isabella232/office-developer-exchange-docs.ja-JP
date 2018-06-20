---
title: 属性 (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: 属性要素は、PersonaType 要素の属性の配列のインスタンスを指定します。
ms.openlocfilehash: 0e800c92c75bf0c475d4bffd33d6ab49f9ad9a9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759465"
---
# <a name="attribution-personaattributiontype"></a>属性 (PersonaAttributionType)

**属性**要素は、 **PersonaType**要素の属性の配列のインスタンスを指定します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ID (文字列)](id-string.md) <br/> |アプリケーションか、ペルソナで、属性を一意に識別する文字列を指定します。  <br/> |
|[SourceId](sourceid.md) <br/> |連絡先または Active Directory の受信者の識別子を指定します。  <br/> |
|[表示名 (文字列)](displayname-string.md) <br/> |フォルダー、連絡先、配布リスト、ユーザーの代理人、またはルールの表示名を定義します。  <br/> |
|[IsWritable](iswritable.md) <br/> |基になっている取引先担当者または Active Directory の受信者に書き込むことがあるかどうかを指定します。  <br/> |
|[IsQuickContact](isquickcontact.md) <br/> |基になっている取引先担当者または Active Directory の受信者は、クイック連絡先かどうかを示すブール値を指定します。  <br/> |
|[IsHidden](ishidden.md) <br/> |かどうか、基になっている取引先担当者または Active Directory の受信者する非表示か、ペルソナの一部として表示を示すブール値が含まれています。  <br/> |
|[フォルダー Id](folderid.md) <br/> |フォルダーの識別子と変更キーが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[帰属 (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) <br/> |1 つまたは複数の連絡先や関連するペルソナに集計される active directory (AD) の受信者の属性情報の配列を指定します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

