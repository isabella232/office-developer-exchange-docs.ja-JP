---
title: RetentionPolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: RetentionPolicyTag 要素は、メールボックス アイテムの保持ポリシーを指定します。
ms.openlocfilehash: 2525f6d7a0ca583342d28dd9f4857a69b3a8c05a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833226"
---
# <a name="retentionpolicytag"></a>RetentionPolicyTag

**RetentionPolicyTag**要素は、メールボックス アイテムの保持ポリシーを指定します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[表示名 (文字列)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [型 (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [説明](description.md) | [IsVisible](isvisible.md)  |  [OptedInto](optedinto.md) | [IsArchive](isarchive.md)
  
### <a name="parent-elements"></a>親要素

[RetentionPolicyTags](retentionpolicytags.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   

