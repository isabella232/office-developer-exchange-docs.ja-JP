---
title: RetentionPolicyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: RetentionPolicyType 要素は、会話内のアイテムに適用される保持ポリシーの種類を指定します。
ms.openlocfilehash: dacb3fa75611cbd6e6e29eab7c791dfd8964c9ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833229"
---
# <a name="retentionpolicytype"></a>RetentionPolicyType

**RetentionPolicyType**要素は、会話内のアイテムに適用される保持ポリシーの種類を指定します。 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 **RetentionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[ConversationAction](conversationaction.md)
  
## <a name="text-value"></a>テキスト値

**RetentionPolicyType**要素のテキスト値は、会話内のアイテムに適用される保持型です。 **削除**のテキスト値は、保持期限が切れると、会話内の項目が削除されることを示します。 **アーカイブ**のテキスト値は、保持期限が切れると、会話内の項目をアーカイブ メールボックスに移動したことを示します。 
  
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
   

