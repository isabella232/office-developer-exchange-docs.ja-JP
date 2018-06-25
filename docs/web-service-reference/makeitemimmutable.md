---
title: MakeItemImmutable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de1d2a60-aeeb-4625-8b11-23c42e1e7bae
description: MakeItemImmutable 要素は、読み取り専用で、項目を行う必要があるかどうかを示すブール値を指定します。
ms.openlocfilehash: 63c05fd3572c7b4ab93fe098d9165a117849ef02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832337"
---
# <a name="makeitemimmutable"></a>MakeItemImmutable

**MakeItemImmutable**要素は、読み取り専用で、項目を行う必要があるかどうかを示すブール値を指定します。 
  
```XML
<MakeItemImmutable>true | false</MakeItemImmutable>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[UpdateItemInRecoverableItems](updateiteminrecoverableitems.md)
  
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **MakeItemImmutable**要素のテキスト値は、項目読み取り専用にすることを示します。 **False**の値は、項目が読み取り/書き込みアクセスを許可していることを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> ||
   

