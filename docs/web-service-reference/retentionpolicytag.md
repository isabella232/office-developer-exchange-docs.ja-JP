---
title: RetentionPolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: RetentionPolicyTag 要素は、メールボックス アイテムのアイテム保持ポリシーを指定します。
ms.openlocfilehash: 58ca3016bed0be625b213a57e5ead1b38a301bfa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524547"
---
# <a name="retentionpolicytag"></a>RetentionPolicyTag

**RetentionPolicyTag** 要素は、メールボックス アイテムのアイテム保持ポリシーを指定します。 
  
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

[DisplayName (string)](displayname-string.md)  | [RetentionId](retentionid.md)  | [RetentionPeriod](retentionperiod.md)  | [Type (ElcFolderType)](type-elcfoldertype.md)  | [RetentionAction](retentionaction.md)  | [説明](description.md)  | [IsVisible](isvisible.md)  | [OptedInto](optedinto.md)  | [IsArchive](isarchive.md)
  
### <a name="parent-elements"></a>親要素

[RetentionPolicyTags](retentionpolicytags.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

