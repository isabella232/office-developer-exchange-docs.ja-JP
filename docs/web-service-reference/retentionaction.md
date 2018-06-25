---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: RetentionAction 要素では、保持タグを持つアイテムに対して実行するアクションを指定します。
ms.openlocfilehash: 54a1038f2e56aad66f89522423ccfbd69dc44a80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833215"
---
# <a name="retentionaction"></a>RetentionAction

**RetentionAction**要素では、保持タグを持つアイテムに対して実行するアクションを指定します。 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 **RetentionActionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>テキスト値

**RetentionAction**要素のテキスト値は、項目に対して実行するアクションです。 次の一覧には、 **RetentionAction**要素のテキスト値が含まれています。 
  
> **なし**- 操作は必要ありませんが、項目に実行されます。 
    
> **MoveToDeletedItems**の項目は、既定の削除済みアイテム フォルダーに移動されます。 
    
> **MoveToFolder**の項目は、指定したフォルダーに移動されます。 
    
> **DeleteAndAllowRecovery**の項目が削除され、大型こみ容器に入れます。 
    
> **PermanentlyDelete**のアイテムはメールボックスから完全に削除します。 
    
> **MarkAsPastRetentionLimit**の項目は、保存期間の制限時間を超過することとしてマークされます。 
    
> **アーカイブに移動**- アイテムは、アーカイブ メールボックスに移動されます。 
    
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
   

