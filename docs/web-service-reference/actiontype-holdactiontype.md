---
title: ActionType (HoldActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f50449b9-e73b-43c5-af96-6433bf434dce
description: ActionType 要素は、保留リストのアクションの種類を示します。
ms.openlocfilehash: 30028da4df2a53a4cd0066823872de5e586020f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546841"
---
# <a name="actiontype-holdactiontype"></a>ActionType (HoldActionType)

**ActionType 要素** は、保留リストのアクションの種類を示します。 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 **HoldActionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>テキスト値

ActionType 要素の **テキスト値** は、メールボックスに設定されたホールドの種類です。 Create のテキスト **値は** 、メールボックスの保持が作成されます。 Update のテキスト **値は** 、メールボックスの保持が更新されるかどうかを示します。 [削除] のテキスト **値は** 、メールボックスの保持が削除されます。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

