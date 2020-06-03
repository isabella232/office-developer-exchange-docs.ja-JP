---
title: ユーザー (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7c42b516-77f6-4aee-99d8-b866d82d793a
description: User 要素は、ユーザー固有の情報を提供します。
ms.openlocfilehash: 8f53319bcf34595305748adafc9aa1e25283611e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530219"
---
# <a name="user-pox"></a>ユーザー (POX)

**User**要素は、ユーザー固有の情報を提供します。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[ユーザー (POX)](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[DisplayName (文字列)](displayname-string.md) <br/> |ユーザーの表示名を表します。  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |従来の識別名でユーザーのメールボックスを識別します。  <br/> |
|[DeploymentId (POX)](deploymentid-pox.md) <br/> |Exchange フォレストを一意に識別します。  <br/> |
|[AutoDiscoverSMTPAddress (POX)](autodiscoversmtpaddress-pox.md) <br/> |自動検出プロセスで使用されるユーザーの SMTP アドレスが含まれます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[応答 (POX)](response-pox.md) <br/> |自動検出サービスからの応答を含みます。  <br/> |
   
## <a name="remarks"></a>注釈

自動検出要求と応答は、UTF-8 でエンコードする必要があります。
  
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

