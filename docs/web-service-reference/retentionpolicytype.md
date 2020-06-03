---
title: RetentionPolicyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: RetentionPolicyType 要素は、スレッド内のアイテムに適用されるアイテム保持ポリシーの種類を指定します。
ms.openlocfilehash: 3900718f10e1e11d5864ebf7e64a3e1e22aa45c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462872"
---
# <a name="retentionpolicytype"></a>RetentionPolicyType

**RetentionPolicyType**要素は、スレッド内のアイテムに適用されるアイテム保持ポリシーの種類を指定します。 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 **RetentionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[ConversationAction](conversationaction.md)
  
## <a name="text-value"></a>テキスト値

**RetentionPolicyType**要素のテキスト値は、会話内のアイテムに適用される保持タイプです。 [**削除**] のテキスト値は、保持保持期間の期限が切れたときにスレッド内のアイテムが削除されることを示します。 **Archive**のテキスト値は、保持保持期間が経過すると、スレッド内のアイテムがアーカイブメールボックスに移動されることを示します。 
  
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
   

