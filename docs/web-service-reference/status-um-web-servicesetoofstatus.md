---
title: 状態 (UM Web サービス - SetOofStatus)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- Status
api_type:
- schema
ms.assetid: 893bcff1-ccdc-493f-b366-ce8a68c813bd
description: Status 要素は、SetOofStatus 操作 (UM Web サービス) 要求で使用する値を定義します。
ms.openlocfilehash: fc4806e4978ae51ec6113ff8fd45da7db223a071
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546939"
---
# <a name="status-um-web-service---setoofstatus"></a>状態 (UM Web サービス - SetOofStatus)

**Status 要素** は [、SetOofStatus 操作 (UM Web サービス)](setoofstatus-operation-um-web-service.md)要求で使用する値を定義します。 
  
[SetOofStatus (UM Web サービス)](setoofstatus-um-web-service.md)
  
[状態 (UM Web サービス - SetOofStatus)](status-um-web-servicesetoofstatus.md)
  
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
|[SetOofStatus (UM Web サービス)](setoofstatus-um-web-service.md) <br/> |要求を行うユーザーのユニファイド メッセージング Office (OOF) 状態を設定する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値が必要です。 指定可能な値は次のいずれかです。
  
- True
    
- False
    
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[SetOofStatus 操作 (UM Web サービス)](setoofstatus-operation-um-web-service.md)

