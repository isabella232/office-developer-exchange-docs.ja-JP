---
title: MailTipsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailTipsEnabled
api_type:
- schema
ms.assetid: 737388b3-7b73-42af-94d3-3dbb0659718f
description: MailTipsEnabled 要素は、メール ヒント サービスが使用可能かどうかを示します。
ms.openlocfilehash: 7444ba7218ebfed85b02dafb0358af9781b22059
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511146"
---
# <a name="mailtipsenabled"></a>MailTipsEnabled

**MailTipsEnabled 要素は**、メール ヒント サービスが使用可能かどうかを示します。 
  
```xml
<MailTipsEnabled>true | false</MailTipsEnabled>
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
|[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |メール ヒント サービスのサービス構成情報が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

メール ヒント サービスが使用可能な **場合、この** 要素のテキスト値は true です。 メール ヒント サービス **が使用** できない場合、この値は false です。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

