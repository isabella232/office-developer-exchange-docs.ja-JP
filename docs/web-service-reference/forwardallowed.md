---
title: ForwardAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc32e0f4-61e9-4c9f-9a03-90a07eb51c53
description: ForwardAllowed 要素は、電子メールの転送が有効になっているかどうかを指定します。
ms.openlocfilehash: 4baa170a531cc9021102ff2255afc113f40e2348
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760586"
---
# <a name="forwardallowed"></a>ForwardAllowed

**ForwardAllowed**要素は、電子メールの転送が有効になっているかどうかを指定します。 
  
```XML
<ForwardAllowed>true | false</ForwardAllowed>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RightsManagementLicenseData](rightsmanagementlicensedata.md) <br/> |権限管理のライセンスについての情報を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **ForwardAllowed**要素のテキスト値は、e メールを転送を許可することを示します。 **False**の値は、転送が許可されていないことを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

