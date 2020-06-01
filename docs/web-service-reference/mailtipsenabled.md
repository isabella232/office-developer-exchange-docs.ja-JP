---
title: Mailヒント有効
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
description: Mailヒント Enabled 要素は、メールヒントサービスが利用可能かどうかを示します。
ms.openlocfilehash: 6be923733f1cbd584010ce5f8ee5b96178d5c2c0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468013"
---
# <a name="mailtipsenabled"></a>Mailヒント有効

**Mailヒント enabled**要素は、メールヒントサービスが利用可能かどうかを示します。 
  
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
|[Mailヒント構成 (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |メールヒントサービスのサービス構成情報が保存されています。  <br/> |
   
## <a name="text-value"></a>テキスト値

メールヒントサービスが利用可能な場合は、この要素のテキスト値は**true**です。 メールヒントサービスが利用できない場合、値は**false**です。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

