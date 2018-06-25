---
title: IsMembershipGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0dc3e285-8f49-48ad-b844-37041c0d782b
description: IsMembershipGroup 要素は、エンティティが、メールボックスまたは配布グループかどうかを示すブール値を指定します。
ms.openlocfilehash: 03ab0dc75d2c798b7f2afeef85aa45f0349be70a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832050"
---
# <a name="ismembershipgroup"></a>IsMembershipGroup

**IsMembershipGroup**要素は、エンティティが、メールボックスまたは配布グループかどうかを示すブール値を指定します。 
  
```XML
<IsMembershipGroup>true | false</IsMembershipGroup>
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
|[SearchableMailbox](searchablemailbox.md) <br/> |メールボックスは、 **GetSearchableMailboxes**要求から返されるかを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **IsMembershipGroup**要素のテキスト値は、エンティティがメールボックスまたは配布グループであることを示します。 False の値は、エンティティが、メールボックスまたは配布グループではないことを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

