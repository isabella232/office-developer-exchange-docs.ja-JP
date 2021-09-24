---
title: MakeItemImmutable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: de1d2a60-aeeb-4625-8b11-23c42e1e7bae
description: MakeItemImmutable 要素は、アイテムを読み取り専用にするかどうかを示すブール値を指定します。
ms.openlocfilehash: 0e1d28f19492bb6dc013957aa5957b59e791b24b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524827"
---
# <a name="makeitemimmutable"></a>MakeItemImmutable

**MakeItemImmutable** 要素は、アイテムを読み取り専用にするかどうかを示すブール値を指定します。 
  
```XML
<MakeItemImmutable>true | false</MakeItemImmutable>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[UpdateItemInRecoverableItems](updateiteminrecoverableitems.md)
  
## <a name="text-value"></a>テキスト値

**MakeItemImmutable 要素のテキスト値が** **true** の場合は、アイテムを読み取り専用にする必要があります。 false の値 **は** 、アイテムが読み取り/書き込みアクセスを許可します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空の場合  <br/> ||
   

