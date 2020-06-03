---
title: 状態 (UM web サービス-SetOofStatus)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 893bcff1-ccdc-493f-b366-ce8a68c813bd
description: Status 要素は、SetOofStatus 操作 (UM web サービス) 要求で使用する値を定義します。
ms.openlocfilehash: 865152baf28c22578664e16db2dcd5f82a04af98
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459981"
---
# <a name="status-um-web-service---setoofstatus"></a>状態 (UM web サービス-SetOofStatus)

**Status**要素は、 [setoofstatus 操作 (UM web サービス)](setoofstatus-operation-um-web-service.md)要求で使用する値を定義します。 
  
[SetOofStatus (UM web サービス)](setoofstatus-um-web-service.md)
  
[状態 (UM web サービス-SetOofStatus)](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
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
|[SetOofStatus (UM web サービス)](setoofstatus-um-web-service.md) <br/> |要求を行ったユーザーのユニファイドメッセージングの不在 (OOF) 状態を設定するための要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値が必要です。 指定可能な値は次のいずれかです。
  
- True
    
- False
    
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[SetOofStatus 操作 (UM web サービス)](setoofstatus-operation-um-web-service.md)

