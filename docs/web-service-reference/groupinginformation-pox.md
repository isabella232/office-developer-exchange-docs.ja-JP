---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: GroupingInformation 要素には、複数のメールボックス間で通知をサブスクライブするときにアフィニティを維持するためにユーザーのメールボックスをグループ化するために使用される値が含まれる。
ms.openlocfilehash: 14e751adcd0b966907ce495a2753b2b26d812a86
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525885"
---
# <a name="groupinginformation-pox"></a>GroupingInformation (POX)

**GroupingInformation** 要素には、複数のメールボックス間で通知をサブスクライブするときにアフィニティを維持するために [](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)ユーザーのメールボックスをグループ化するために使用される値が含まれる。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[GroupingInformation (POX)](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |クライアントをサーバーに接続するための仕様Exchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、他のメールボックスの **GroupingInformation** 要素の値と比較されます。 同じ値を持ち、Web サービス (EWS) エンドポイントExchange同じ値を使用するメールボックスは、アフィニティを維持するためにグループ化できます。 詳細については、「サブスクリプションのグループ[と](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)メールボックス サーバー間のアフィニティを維持する」を参照Exchange。
  
## <a name="remarks"></a>注釈

**GroupingInformation** 要素は、**値** が ["EXPR" の Type (POX)](type-pox.md)子要素を持つ Protocol 要素にのみ適用できます。 
  
## <a name="see-also"></a>関連項目

- [POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)
- [サブスクリプション グループと Exchange のメールボックス サーバー間のアフィニティを維持する](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

