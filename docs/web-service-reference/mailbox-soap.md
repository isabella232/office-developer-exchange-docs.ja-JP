---
title: メールボックス (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4ad59e5b-4047-4c34-a318-ca06c31d3de8
description: メールボックスの要素には、検出対象のユーザーの電子メール アドレスが含まれています。
ms.openlocfilehash: b98397dadf8c467031eb8febe9732d4e426372e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832253"
---
# <a name="mailbox-soap"></a>メールボックス (SOAP)

**メールボックス**の要素には、検出対象のユーザーの電子メール アドレスが含まれています。 
  
```XML
<Mailbox/>
```

**string**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ユーザー (SOAP)](user-soap.md) <br/> |1 人のユーザーの id を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**メールボックス**要素のテキスト値は、検出対象のユーザーの電子メール アドレスです。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)

