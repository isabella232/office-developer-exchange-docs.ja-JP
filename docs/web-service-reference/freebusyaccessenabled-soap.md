---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: FreeBusyAccessEnabled 要素は、FreeBusyAccessEnabled () フラグを表します。 FreeBusyAccessEnabled 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: c148d8fa1301339f8579884dc02b6c9e452f3035
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461297"
---
# <a name="freebusyaccessenabled-soap"></a>FreeBusyAccessEnabled (SOAP)

**FreeBusyAccessEnabled**要素は、 **FreeBusyAccessEnabled ()** フラグを表します。 **FreeBusyAccessEnabled**要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。 
  
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
|[組織のリレーションシップ設定 (SOAP)](organizationrelationshipsettings-soap.md) <br/> |1つの組織の組織上の関係のリストを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**FreeBusyAccessEnabled**要素のテキスト値が**true**の場合は、共有関係を使用して、組織内のユーザーから空き時間情報を取得する必要があることを示します。 値が**false**の場合は、共有リレーションシップを抑制する必要があることを示します。 
  
## <a name="remarks"></a>注釈

この要素を使用して、サーバーからの空き時間情報を許可または抑制します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[Get組織の Relationshipsettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

