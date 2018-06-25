---
title: ファイアウォール (HoldActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f50449b9-e73b-43c5-af96-6433bf434dce
description: ファイアウォールの要素では、保留リストの動作の種類を示します。
ms.openlocfilehash: cb1cfa8a1306c4a6cacf5c82824d19cab57e7941
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759268"
---
# <a name="actiontype-holdactiontype"></a>ファイアウォール (HoldActionType)

**ファイアウォール**の要素では、保留リストの動作の種類を示します。 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 **HoldActionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>テキスト値

**ファイアウォール**の要素のテキスト値は、保留中のメールボックスの設定の種類です。 **作成する**テキスト値は、メールボックスの保留リストを作成することを示します。 **更新プログラム**のテキスト値は、メールボックスの保留リストを更新することを示します。 **削除**のテキスト値は、メールボックスの保持を削除することを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

