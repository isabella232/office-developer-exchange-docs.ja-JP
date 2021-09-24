---
title: SettingName (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 8bcb0411-58b0-4e37-b97e-00c07dcbecb1
description: SettingName 要素は、応答内の設定の名前を表します。
ms.openlocfilehash: 1a676f55ad86496ae8bdbdfbeaeb9827b1aa6646
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531882"
---
# <a name="settingname-soap"></a>SettingName (SOAP)

**SettingName 要素** は、応答内の設定の名前を表します。 
  
```XML
<SettingName/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |ユーザー設定の取得中に返されるエラーを表します。  <br/> |
|[DomainSettingError (SOAP)](domainsettingerror-soap.md) <br/> |ドメイン設定の取得中に発生したエラーを表します。 これは **、GetDomainSettings 要求からのエラーを表** します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**SettingName** 要素の値は、応答内の設定の名前を表します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |はい  <br/> |
   

