---
title: IncludePersonalArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b373bb1a-6b1d-4959-98a1-4c4ea62973bc
description: IncludePersonalArchive 要素は、個人用アーカイブを検索に含めるかどうかを指定します。
ms.openlocfilehash: 2567475fbb2542c7d01e651f2d348f6f91d50b78
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547219"
---
# <a name="includepersonalarchive"></a>IncludePersonalArchive

**IncludePersonalArchive 要素は**、個人用アーカイブを検索に含めるかどうかを指定します。 
  
```XML
<IncludePersonalArchive>true | false</IncludePersonalArchive>
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

**IncludePersonalArchive** 要素のテキスト値 **true** は、個人用アーカイブが検索に含まれているかどうかを示します。 false の **値は** 、個人用アーカイブが検索に含まれていないかどうかを示します。 
  
## <a name="remarks"></a>注釈

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

