---
title: MailTipsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsEnabled
api_type:
- schema
ms.assetid: 737388b3-7b73-42af-94d3-3dbb0659718f
description: MailTipsEnabled 要素は、メール ヒントのサービスが利用可能かどうかを示します。
ms.openlocfilehash: 4fe2cae1087ab667133ec685c3325b14c4f12088
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832330"
---
# <a name="mailtipsenabled"></a>MailTipsEnabled

**MailTipsEnabled**要素は、メール ヒントのサービスが利用可能かどうかを示します。 
  
```xml
<MailTipsEnabled>true | false</MailTipsEnabled>
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
|[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |メール ヒント サービスのサービスの構成情報が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

**メール ヒントのサービスがある場合はこの要素のテキスト値は** 値は、メール ヒントのサービスが利用できない場合**は false** 。 
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

