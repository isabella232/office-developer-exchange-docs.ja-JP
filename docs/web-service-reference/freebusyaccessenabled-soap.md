---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: FreeBusyAccessEnabled 要素は、FreeBusyAccessEnabled() フラグを表します。 FreeBusyAccessEnabled 要素は内部でのみ使用できます。 この要素は、クライアントでは使用されません。
ms.openlocfilehash: faf51798ba211b4219a3f2abee3b3e5e9ce4ab29
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530219"
---
# <a name="freebusyaccessenabled-soap"></a>FreeBusyAccessEnabled (SOAP)

**FreeBusyAccessEnabled 要素** は **、FreeBusyAccessEnabled() フラグを表** します。 **FreeBusyAccessEnabled 要素** は内部でのみ使用できます。 この要素は、クライアントでは使用されません。 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
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
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |1 つの組織の組織関係の一覧を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**FreeBusyAccessEnabled** 要素のテキスト値 **が true** の場合は、共有関係を使用して組織内のユーザーから空き時間情報を取得する必要があります。 false の **値は** 、共有関係を抑制する必要があります。 
  
## <a name="remarks"></a>注釈

この要素を使用して、サーバーからの空き時間情報を許可または抑制します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

