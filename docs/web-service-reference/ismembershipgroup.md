---
title: Isメンバーシップグループ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0dc3e285-8f49-48ad-b844-37041c0d782b
description: Isメンバーシップグループ要素は、エンティティが配布グループまたはメールボックスであるかどうかを示すブール値を指定します。
ms.openlocfilehash: ed79961c6d13ab226c0b489103ef3d2c4a08668d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459287"
---
# <a name="ismembershipgroup"></a>Isメンバーシップグループ

**Isメンバーシップグループ**要素は、エンティティが配布グループまたはメールボックスであるかどうかを示すブール値を指定します。 
  
```XML
<IsMembershipGroup>true | false</IsMembershipGroup>
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
|[SearchableMailbox](searchablemailbox.md) <br/> |**Getsearchablemailboxes**要求から返されるメールボックスを指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Isメンバーシップグループ**要素のテキスト値が**true**である場合は、エンティティが配布グループまたはメールボックスであることを示します。 値が false の場合、エンティティが配布グループまたはメールボックスではないことを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

