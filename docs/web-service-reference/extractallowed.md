---
title: ExtractAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bc213f0e-a655-44e9-9ac9-bc1673bae1fe
description: ExtractAllowed 要素は、エンティティ抽出を有効にするかどうかを指定します。
ms.openlocfilehash: a51adaba24ef6ee285acf786398d6e6cdfbfee35
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535328"
---
# <a name="extractallowed"></a>ExtractAllowed

**ExtractAllowed 要素** は、エンティティ抽出を有効にするかどうかを指定します。 
  
```XML
<ExtractAllowed>true | false</ExtractAllowed
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
|[RightsManagementLicenseData](rightsmanagementlicensedata.md) <br/> |権限管理ライセンスに関する情報を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**ExtractAllowed** 要素の **テキスト値が true** の場合は、エンティティの抽出が有効になっているかどうかを示します。 false の値 **は** 、エンティティの抽出が有効になっていない状態を示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

