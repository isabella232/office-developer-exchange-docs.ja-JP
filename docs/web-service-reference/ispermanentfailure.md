---
title: IsPermanentFailure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: IsPermanentFailure 要素は、アイテムのインデックスを作成する以前の試行が失敗したかどうかを示します。
ms.openlocfilehash: e5ed20de3c3de9c39d1487e3177c1b6ec358d990
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532721"
---
# <a name="ispermanentfailure"></a>IsPermanentFailure

**IsPermanentFailure** 要素は、アイテムのインデックスを作成する以前の試行が失敗したかどうかを示します。 
  
```XML
<IsPermanentFailure>true | false</IsPermanentFailure>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[NonIndexableItemDetail](nonindexableitemdetail.md)
  
## <a name="text-value"></a>テキスト値

**IsPermanentFailure** 要素のテキスト値 **が true** の場合、メールボックス アイテムのインデックスを作成する以前の試行が失敗しました。 false の **値は** 、メールボックス アイテムのインデックスを作成する以前の試行が成功したかどうかを示します。 
  
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
   

