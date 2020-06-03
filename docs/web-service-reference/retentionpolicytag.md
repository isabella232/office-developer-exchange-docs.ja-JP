---
title: New-retentionpolicytag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: New-retentionpolicytag 要素は、メールボックスアイテムのアイテム保持ポリシーを指定します。
ms.openlocfilehash: 3ece841e14e6cf11ab15e4a4d8b83a778ae32e46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465178"
---
# <a name="retentionpolicytag"></a>New-retentionpolicytag

**New-retentionpolicytag**要素は、メールボックスアイテムのアイテム保持ポリシーを指定します。 
  
```XML
<RetentionPolicyTag>
   <DisplayName/>
   <RetentionId/>
   <RetentionPeriod/>
   <Type/>
   <RetentionAction/>
   <Description/>
   <IsVisible/>
   <OptedInto/>
   <IsArchive/>
</RetentionPolicyTag>
```

 **RetentionPolicyTagType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[DisplayName (文字列)](displayname-string.md)  | [RetentionId](retentionid.md)  | [保存期間](retentionperiod.md)  | [Type (ElcFolderType)](type-elcfoldertype.md)  | [Retentionaction](retentionaction.md)  | [説明](description.md)  | [IsVisible](isvisible.md)  | [Optedinto](optedinto.md)  | [Isarchive](isarchive.md)
  
### <a name="parent-elements"></a>親要素

[RetentionPolicyTags](retentionpolicytags.md)
  
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
   

