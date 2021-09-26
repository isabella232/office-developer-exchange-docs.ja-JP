---
title: ExpandGroupMembership
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: ExpandGroupMembership 要素は、GetSearchableMailboxes 要求から返されるグループのメンバーシップを拡張するかどうかを示します。
ms.openlocfilehash: fb835f8f1fa9fb957c6b3bf3ddef80e68d9c049f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541400"
---
# <a name="expandgroupmembership"></a>ExpandGroupMembership

**ExpandGroupMembership** 要素は **、GetSearchableMailboxes** 要求から返されるグループのメンバーシップを拡張するかどうかを示します。 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md)  | [GetSearchableMailboxes](getsearchablemailboxes.md)
  
## <a name="text-value"></a>テキスト値

**ExpandGroupElement 要素のテキスト値が** **true** の場合、グループ メンバーシップが展開されます。 false の **値は** 、グループのメンバーを表示するためにグループ メンバーシップが展開されていない状態を示します。 
  
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
   

