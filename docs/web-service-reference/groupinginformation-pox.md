---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: GroupingInformation 要素には、複数のメールボックス間での通知にサブスクライブしているときに、アフィニティを維持するためにユーザーのメールボックスをグループ化するために使用される値が含まれています。
ms.openlocfilehash: bcde002c794ac79d9515befc0755c1f954ee8706
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831781"
---
# <a name="groupinginformation-pox"></a>GroupingInformation (POX)

**GroupingInformation**要素には、複数のメールボックスの間で、通知を購読する場合は、[アフィニティを維持](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)するためにユーザーのメールボックスをグループ化するために使用される値が含まれています。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
[GroupingInformation (POX)](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントを Exchange サーバーに接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、他のメールボックスの**GroupingInformation**要素の値と比較されます。 メールボックスを同じ値を持つし、同一の Exchange Web サービス (EWS) のエンドポイントを使用してグループ化できるアフィニティを維持するためにします。 詳細については、 [Exchange でのサブスクリプションのグループとメールボックス サーバー間のアフィニティを維持](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)を参照してください。
  
## <a name="remarks"></a>備考

**GroupingInformation**要素では、EXPR の値を持つ[型 (POX)](type-pox.md)の子要素を持つ**プロトコル**要素に該当する場合のみ。 
  
## <a name="see-also"></a>関連項目

- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)
- [Exchange の購読グループとメールボックス サーバー間のアフィニティを維持します。](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

