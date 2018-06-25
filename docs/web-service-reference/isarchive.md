---
title: IsArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b89d8a78-5c18-4547-aaf4-4b16a93190a7
description: IsArchive 要素は、メールボックスが、アーカイブ メールボックスであるかどうかを示すブール値を指定します。
ms.openlocfilehash: 417afd1afc25e5872d1f511feff34494fe6b7b62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831990"
---
# <a name="isarchive"></a>IsArchive

**IsArchive**要素は、メールボックスが、アーカイブ メールボックスであるかどうかを示すブール値を指定します。 
  
```XML
<IsArchive>true | false</IsArchive>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[FailedMailbox](failedmailbox.md) | [RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>テキスト値

テキストの値**は true** **IsArchive**要素の移動先のメールボックスが、アーカイブ メールボックスであることを示します。 **False**の値は、移動先のメールボックスは、アーカイブ メールボックスではないことを示します。 
  
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

