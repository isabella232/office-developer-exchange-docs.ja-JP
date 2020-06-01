---
title: IsExternalMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5cc83174-e684-42c8-b72a-f82d3de3bb2f
description: IsExternalMailbox 要素は、メールボックスが組織の外部にあるかどうかを示します。
ms.openlocfilehash: 9be702b05e89857913023a8ec34b78ea4c309274
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455290"
---
# <a name="isexternalmailbox"></a>IsExternalMailbox

**IsExternalMailbox**要素は、メールボックスが組織の外部にあるかどうかを示します。 
  
```XML
<IsExternalMailbox>true | false</IsExternalMailbox>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SearchableMailbox](searchablemailbox.md)
  
## <a name="text-value"></a>テキスト値

**IsExternalMailbox**要素のテキスト値が**true の場合**は、メールボックスが外部組織にあることを示します。 値が**false**の場合は、メールボックスが組織内にあることを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

