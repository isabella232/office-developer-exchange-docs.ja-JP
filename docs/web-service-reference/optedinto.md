---
title: OptedInto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 083a23d9-acc3-4c15-9d30-c20bf7e6808d
description: OptedInto 要素は、ユーザーがアイテム保持ポリシーにオプトインしたかどうかを示すブール値を指定します。
ms.openlocfilehash: 6dbfe898ad6eb3141b265d51c8ec0cb830916a9d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518065"
---
# <a name="optedinto"></a>OptedInto

**OptedInto** 要素は、ユーザーがアイテム保持ポリシーにオプトインしたかどうかを示すブール値を指定します。 
  
```XML
<OptedInto>true | false</OptedInto>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>テキスト値

**OptedInto** 要素のテキスト値 **が true** の場合は、ユーザーがアイテム保持ポリシーにオプトインすることを示します。 false の **値は** 、ユーザーがアイテム保持ポリシーを選択しなかったことを示します。 
  
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
   

