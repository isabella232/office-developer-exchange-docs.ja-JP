---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: GroupingInformation 要素には、ユーザーのメールボックスをグループ化して、複数のメールボックス間で通知をサブスクライブするときのアフィニティを維持するために使用される値が含まれています。
ms.openlocfilehash: 7cab5d68f7dd5ec1f6caded5b9da6cfee03f3a67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530079"
---
# <a name="groupinginformation-pox"></a>GroupingInformation (POX)

**Groupinginformation**要素には、ユーザーのメールボックスをグループ化して、複数のメールボックス間で通知をサブスクライブするときの[アフィニティを維持](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)するために使用される値が含まれています。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[プロトコル (POX)](protocol-pox.md)
  
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
|[プロトコル (POX)](protocol-pox.md) <br/> |クライアントを Exchange サーバーに接続するための仕様が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、他のメールボックスの**Groupinginformation**要素の値と比較されます。 同じ値を持つメールボックスは、同じ Exchange Web サービス (EWS) エンドポイントを使用して、アフィニティを維持するためにまとめてグループ化することができます。 詳細については、「 [Exchange のサブスクリプショングループとメールボックスサーバー間のアフィニティを維持する](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)」を参照してください。
  
## <a name="remarks"></a>注釈

**Groupinginformation**要素は、値が "EXPR" である[Type (POX)](type-pox.md)子要素を持つ**プロトコル**要素にのみ適用されます。 
  
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)
- [サブスクリプション グループと Exchange のメールボックス サーバー間のアフィニティを維持する](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

