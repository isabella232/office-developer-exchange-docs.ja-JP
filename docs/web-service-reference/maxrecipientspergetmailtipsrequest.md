---
title: Max受信者 Spergetmailヒント要求
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxRecipientsPerGetMailTipsRequest
api_type:
- schema
ms.assetid: 8ff5df18-1989-4217-b4c0-599232911d0c
description: Max受信者 Spergetmailヒント要求要素は、Getメールヒント操作に渡すことができる受信者の最大数を示します。
ms.openlocfilehash: cec343182b364fce040d5e32928cbeb569a22124
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468405"
---
# <a name="maxrecipientspergetmailtipsrequest"></a>Max受信者 Spergetmailヒント要求

**Max受信者 Spergetmailヒント要求**要素は、 [getメールヒント操作](getmailtips-operation.md)に渡すことができる受信者の最大数を示します。
  
```XML
<MaxRecipientsPerGetMailTipsRequest/>
```

 **int**
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

テキスト値は、 [Getmailtips ヒント操作](getmailtips-operation.md)に渡すことができる受信者の最大数を表す整数です。
  
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



[GetMailTips ヒント操作](getmailtips-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

