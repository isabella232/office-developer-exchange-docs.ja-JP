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
description: SetPlayOnPhoneDialString 要素は、PlayOnPhone 操作 (UM web サービス) の既定のダイヤル文字列を設定するための要求および PlayOnPhoneGreeting (UM web サービス) の操作の要求を定義します。
ms.openlocfilehash: fd82dc6ef0dd90a2318da93191f657005b7a5c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833450"
---
# <a name="setplayonphonedialstring-um-web-service"></a>SetPlayOnPhoneDialString (UM web サービス)

**SetPlayOnPhoneDialString**要素は、 [PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)および[PlayOnPhoneGreeting 操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)の要求の既定のダイヤル文字列を設定する要求を定義します。 
  
[SetPlayOnPhoneDialString (UM web サービス)](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 **complexType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[dialString (UM web サービス)](dialstring-um-web-service.md) <br/> |ダイヤルの既定の文字列として設定するのには電話番号です。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[SetPlayOnPhoneDialString 操作 (UM web サービス)](setplayonphonedialstring-operation-um-web-service.md)

