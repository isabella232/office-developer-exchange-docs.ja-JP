---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: RetentionAction 要素は、保持タグを持つアイテムに対して実行されるアクションを指定します。
ms.openlocfilehash: c16988413e732ddc3cd6ebc355cb73c4d96550c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465234"
---
# <a name="retentionaction"></a>RetentionAction

**Retentionaction**要素は、保持タグを持つアイテムに対して実行されるアクションを指定します。 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 **RetentionActionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[New-retentionpolicytag](retentionpolicytag.md)
  
## <a name="text-value"></a>テキスト値

**Retentionaction**要素のテキスト値は、アイテムに対して実行されるアクションです。 次の一覧に、 **Retentionaction**要素のテキスト値を示します。 
  
> **None** -アイテムに対してアクションは実行されません。 
    
> **MoveToDeletedItems** -アイテムは既定の削除済みアイテムフォルダーに移動されます。 
    
> **Movetofolder** -アイテムは指定されたフォルダーに移動されます。 
    
> **Deleteandallowrecovery** -アイテムが削除され、[収集] に入ります。 
    
> **PermanentlyDelete** -アイテムはメールボックスから完全に削除されます。 
    
> **MarkAsPastRetentionLimit** -アイテムは、保持時間制限を超えたとしてマークされています。 
    
> **Movetoarchive** -アイテムはアーカイブメールボックスに移動されます。 
    
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
   

