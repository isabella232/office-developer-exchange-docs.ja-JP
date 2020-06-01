---
title: ImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 556457d5-a730-4131-853f-1198c27c5942
description: ImItemList 要素には、インスタントメッセージンググループとインスタントメッセージングの連絡先の一覧が含まれています。
ms.openlocfilehash: 976897fd999b61207a94a8b1dc60cc1b1308acd8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460674"
---
# <a name="imitemlist"></a>ImItemList

**Imitemlist**要素には、インスタントメッセージンググループとインスタントメッセージングの連絡先の一覧が含まれています。 
  
```XML
<ImItemList>
   <Groups/>
   <Personas/>
</ImItemList>
```

 **ImItemListType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[グループ (ArrayOfImGroupType)](groups-arrayofimgrouptype.md)  | [ペルソナ](personas-ex15websvcsotherref.md)
  
### <a name="parent-elements"></a>親要素

[Getimitemsresponse](getimitemsresponse.md)  | [Getimitemlistresponse](getimitemlistresponse.md)
  
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
   

