---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: FreeBusyAccessEnabled 要素は、FreeBusyAccessEnabled() フラグを表します。 FreeBusyAccessEnabled 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 4727e7054c02a4b5d454cb880691ecc01a075327
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760599"
---
# <a name="freebusyaccessenabled-soap"></a>FreeBusyAccessEnabled (SOAP)

**FreeBusyAccessEnabled**要素は、 **FreeBusyAccessEnabled()** フラグを表します。 **FreeBusyAccessEnabled**要素は、内部使用のみ。 クライアントでは、この要素は使用されません。 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
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
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |1 つの組織の組織との関係のリストを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **FreeBusyAccessEnabled**要素のテキスト値は、組織内のユーザーの空き時間情報を取得するために共有を使用することを示します。 **False**の値は、共有関係を抑制するかを示します。 
  
## <a name="remarks"></a>備考

許可するか、サーバーから空き時間情報が表示されないようにするには、この要素を使用します。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

