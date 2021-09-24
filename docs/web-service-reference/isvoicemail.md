---
title: IsVoicemail
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsVoicemail
api_type:
- schema
ms.assetid: 96d81d6e-4b75-43ad-b151-2dd4fd57db94
description: IsVoicemail 要素は、条件または例外を適用するために、受信メッセージがボイス メール メッセージである必要かどうかを示します。
ms.openlocfilehash: df7233f282d9b6b2e5a0833aef389cc50614d986
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522846"
---
# <a name="isvoicemail"></a>IsVoicemail

**IsVoicemail 要素** は、条件または例外を適用するために、受信メッセージがボイス メール メッセージである必要かどうかを示します。 
  
```XML
<IsVoicemail>true | false</IsVoicemail>
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
|[条件](conditions.md) <br/> |満たされると、ルールのルール アクションをトリガーする条件を表します。  <br/> |
|[例外](exceptions.md) <br/> |受信トレイ ルールで使用可能なすべてのルール例外条件を表す例外を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

true のテキスト **値は** 、条件または例外が適用されるには、メッセージがボイス メール メッセージである必要があります。 false の **値は** 、条件または例外が適用されるには、メッセージがボイス メール メッセージでなくする必要があります。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

