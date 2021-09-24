---
title: IncludeUnsearchableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9a9bd2dc-f5b9-4b82-a6a0-f643d2951080
description: IncludeUnsearchableItems 要素は、検索できないアイテムを含めるかどうかを指定します。
ms.openlocfilehash: 3bffd68c20623aa4c63dd295d8b4619999c1d4a5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533105"
---
# <a name="includeunsearchableitems"></a>IncludeUnsearchableItems

**IncludeUnsearchableItems** 要素は、検索できないアイテムを含めるかどうかを指定します。 
  
```XML
<IncludeUnsearchableItems>true | false</IncludeUnsearchableItems>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindMailboxStatisticsByKeywords](findmailboxstatisticsbykeywords.md) <br/> |キーワードによってメールボックスの統計情報を検索する要求を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**IncludeUnsearchableItems** 要素のテキスト値 **が true** の場合、検索できないアイテムの統計情報は含まれません。 false の **値は** 、検索できないアイテムの統計情報が含まれるかどうかを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

