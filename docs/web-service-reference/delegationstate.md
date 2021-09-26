---
title: DelegationState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DelegationState
api_type:
- schema
ms.assetid: 9dbb83ed-1ded-48f3-8e06-2489fc8b28d5
description: DelegateState 要素は、委任されたタスクの状態を表します。
ms.openlocfilehash: 218e96b73c1681bd9bb2fd964a735b62b9e2a94b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542506"
---
# <a name="delegationstate"></a>DelegationState

**DelegateState 要素** は、委任されたタスクの状態を表します。 
  
```xml
<DelegationState/>
```

**TaskDelegateStateType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[タスク](task.md) <br/> |ストア内のタスクをExchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

これは読み取り専用プロパティです。 指定可能な値は次のいずれかです。
  
- NoMatch
    
- OwnNew
    
- Owned (所有)
    
- Accepted
    
- 拒否
    
- Max
    
## <a name="remarks"></a>注釈

Exchange2007 Microsoft Exchange Server Web サービスでは、タスクの割り当てがサポートされていません。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

