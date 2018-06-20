---
title: IncludeUnsearchableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a9bd2dc-f5b9-4b82-a6a0-f643d2951080
description: IncludeUnsearchableItems 要素を検索できない項目を含めるかどうかを指定します。
ms.openlocfilehash: 4c6b9b3752330bf914c9901d2e8f69e93546fec6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831907"
---
# <a name="includeunsearchableitems"></a>IncludeUnsearchableItems

**IncludeUnsearchableItems**要素を検索できない項目を含めるかどうかを指定します。 
  
```XML
<IncludeUnsearchableItems>true | false</IncludeUnsearchableItems>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindMailboxStatisticsByKeywords](findmailboxstatisticsbykeywords.md) <br/> |キーワードでメールボックスの統計情報を検索するための要求を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **IncludeUnsearchableItems**要素のテキスト値は、統計情報が検索可能ではない項目に含まれていないことを示します。 **False**の値は、統計情報は、検索可能ではない項目に含まれていることを示します。 
  
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
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

