---
title: NonIndexableItemDetail
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a26d4c02-f1bd-40c4-9257-5db45e839f17
description: NonIndexableItemDetail 要素は、インデックスを作成できないアイテムに関する詳細情報を指定します。
ms.openlocfilehash: 4fc4324501570402d22aa303d6af2a60b50b3cc6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466739"
---
# <a name="nonindexableitemdetail"></a>NonIndexableItemDetail

**Nonindexableitemdetail**要素は、インデックスを作成できないアイテムに関する詳細情報を指定します。 
  
```XML
<NonIndexableItemDetail>
   <ItemId/>
   <ErrorCode/>
   <ErrorDescription/>
   <IsPartiallyIndexed/>
   <IsPermanentFailure/>
   <SortValue/>
   <AttemptCount/>
   <LastAttemptTime/>
   <AdditionalInfo/>
</NonIndexableItemDetail>
```

 **Nonindexableitemの種類**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ItemId](itemid.md)  | [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md)  | [ErrorDescription](errordescription.md)  | [Ispartiのインデックス付き](ispartiallyindexed.md)  | [IsPermanentFailure](ispermanentfailure.md)  | [Sortvalue](sortvalue.md)  | [AttemptCount](attemptcount.md)  | [LastAttemptTime](lastattempttime.md)  | [Additionalinfo](additionalinfo.md)
  
### <a name="parent-elements"></a>親要素

[アイテム (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

