---
title: RetentionPolicyTags
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8ed4a48a-d510-4cbe-a172-145c33ffb297
description: RetentionPolicyTags 要素には、GetUserRetentionPolicyTags WSDL 操作の応答で返される保持タグの一覧が含まれます。
ms.openlocfilehash: 9bd41a0826aff38e8fc2420553d4c7527c5a8e33
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524533"
---
# <a name="retentionpolicytags"></a>RetentionPolicyTags

**RetentionPolicyTags** 要素には **、GetUserRetentionPolicyTags** WSDL 操作の応答で返される保持タグの一覧が含まれます。 
  
```XML
<RetentionPolicyTags>
   <RetentionPolicyTag/>
</RetentionPolicyTags>
```

 **ArrayOfRetentionPolicyTagsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[RetentionPolicyTag](retentionpolicytag.md)
  
### <a name="parent-elements"></a>親要素

[GetUserRetentionPolicyTagsResponse](getuserretentionpolicytagsresponse.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

