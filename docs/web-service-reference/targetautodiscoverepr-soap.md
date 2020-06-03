---
title: TargetAutodiscoverEpr (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: fdb9cc7a-cf0a-431b-9f6f-5f1db1792db7
description: TargetAutodiscoverEpr 要素は、TargetAutodiscoverEpr プロパティを表します。 TargetAutodiscoverEpr 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: f8609f61021d5701f7a8fa2590a85824caf296c6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530290"
---
# <a name="targetautodiscoverepr-soap"></a>TargetAutodiscoverEpr (SOAP)

**TargetAutodiscoverEpr**要素は、 **TargetAutodiscoverEpr**プロパティを表します。 **TargetAutodiscoverEpr**要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。 
  
```XML
<TargetAutodiscoverEpr/>
```

 **anyURI**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[組織のリレーションシップ設定 (SOAP)](organizationrelationshipsettings-soap.md) <br/> |1つの組織の組織上の関係のリストを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、組織上の関係の uniform resource identifier (URI) です。
  
## <a name="remarks"></a>注釈

この要素は、外部組織のサーバーの自動検出 URL を指定します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[Get組織の Relationshipsettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

