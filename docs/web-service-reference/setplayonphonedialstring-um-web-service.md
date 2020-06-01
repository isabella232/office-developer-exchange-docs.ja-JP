---
title: SetPlayOnPhoneDialString (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: 513a5072-c3ac-405f-98c2-0ab982d0a360
description: SetPlayOnPhoneDialString 要素は、PlayOnPhone 操作 (UM web サービス) および Playonphone 案内応答操作 (UM web サービス) 要求の既定のダイヤル文字列を設定するための要求を定義します。
ms.openlocfilehash: 40021e9dedafb5fafda91bf3612d8a6485dae8e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458629"
---
# <a name="setplayonphonedialstring-um-web-service"></a>SetPlayOnPhoneDialString (UM web サービス)

**SetPlayOnPhoneDialString**要素は、 [playonphone 操作 (um web サービス)](playonphone-operation-um-web-service.md)および[playonphone 案内応答操作 (um web サービス)](playonphonegreeting-operation-um-web-service.md)要求の既定のダイヤル文字列を設定するための要求を定義します。 
  
[SetPlayOnPhoneDialString (UM web サービス)](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 **complexType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[[] (UM web サービス)](dialstring-um-web-service.md) <br/> |既定のダイヤル文字列として設定する電話番号です。  <br/> |
   
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



[SetPlayOnPhoneDialString 操作 (UM web サービス)](setplayonphonedialstring-operation-um-web-service.md)

