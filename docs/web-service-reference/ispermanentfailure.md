---
title: IsPermanentFailure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: IsPermanentFailure 要素は、アイテムに対する以前のインデックス作成の試行が失敗したかどうかを示します。
ms.openlocfilehash: 48a13eebfa16c538c1b10d92f080d51f1b318d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460394"
---
# <a name="ispermanentfailure"></a>IsPermanentFailure

**IsPermanentFailure**要素は、アイテムに対する以前のインデックス作成の試行が失敗したかどうかを示します。 
  
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

**IsPermanentFailure**要素のテキスト値が**true**になっている場合、メールボックスアイテムの以前のインデックス作成の試行が失敗したことを示します。 値が**false**の場合、メールボックスアイテムの以前のインデックス作成が成功したことを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

