---
title: Playon電話応答メッセージ (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 43eda596-3609-4e1b-8502-1db2636535cf
description: Playonphone 案内応答要素は、電話でユニファイドメッセージングの応答メッセージを再生するための要求を定義します。
ms.openlocfilehash: 197e4ba671e1711b73b1e7c239339db589357581
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529925"
---
# <a name="playonphonegreeting-um-web-service"></a>Playon電話応答メッセージ (UM web サービス)

**Playonphone 案内応答**要素は、電話でユニファイドメッセージングの応答メッセージを再生するための要求を定義します。 
  
[Playon電話応答メッセージ (UM web サービス)](playonphonegreeting-um-web-service.md)
  
```xml
<PlayOnPhoneGreeting>
  <GreetingType/>
  <DialString/>
</PlayOnPhoneGreeting>
```

 **complexType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[GreetingType (UM web サービス)](greetingtype-um-web-service.md) <br/> |[Playon電話案内応答操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)要求で使用する案内応答の種類を定義します。  <br/> |
|[[] (UM web サービス)](dialstring-um-web-service.md) <br/> |ダイヤルする電話番号の値が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[Playon電話案内応答操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)

