---
title: IsUMEnabled (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: 33810bbd-837f-4a71-9ed9-cb4b8c52186d
description: IsUMEnabled 要素は、メールボックスがユニファイドメッセージングに対して有効になっているかどうかを示します。
ms.openlocfilehash: ea5bde677c62664acad8afd5c8142e96d82b7a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458230"
---
# <a name="isumenabled-um-web-service"></a>IsUMEnabled (UM web サービス)

**IsUMEnabled**要素は、メールボックスがユニファイドメッセージングに対して有効になっているかどうかを示します。 
  
```xml
<IsUMEnabled/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

この要素が含まれている場合は、ブール値を表すテキスト値が必要です。 値が**true**の場合は、メールボックスがユニファイドメッセージングに対して有効になっていることを示します。 値が**false**の場合は、メールボックスがユニファイドメッセージングに対して有効になっていないことを意味します。 
  
## <a name="remarks"></a>注釈

メールボックスがユニファイドメッセージングに対して有効になっているかどうかを確認するには、 [IsUMEnabled 操作 (UM web サービス)](isumenabled-operation-um-web-service.md)を使用します。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[IsUMEnabled 操作 (UM web サービス)](isumenabled-operation-um-web-service.md)


[Exchange 用のユニファイドメッセージング web サービスの XML 要素](unified-messaging-web-service-xml-elements-for-exchange.md)

