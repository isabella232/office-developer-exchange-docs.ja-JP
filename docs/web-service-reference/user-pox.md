---
title: User (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 7c42b516-77f6-4aee-99d8-b866d82d793a
description: User 要素は、ユーザー固有の情報を提供します。
ms.openlocfilehash: 832e0a63e75a08406b3aa397ac29ad5aa300cfe0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522408"
---
# <a name="user-pox"></a>User (POX)

**User 要素は**、ユーザー固有の情報を提供します。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[User (POX)](user-pox.md)
  
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
|[DisplayName (string)](displayname-string.md) <br/> |ユーザーの表示名を表します。  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |従来の識別名でユーザーのメールボックスを識別します。  <br/> |
|[DeploymentId (POX)](deploymentid-pox.md) <br/> |フォレストを一意にExchangeします。  <br/> |
|[AutoDiscoverSMTPAddress (POX)](autodiscoversmtpaddress-pox.md) <br/> |自動検出プロセスに使用されるユーザーの SMTP アドレスを格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Response (POX)](response-pox.md) <br/> |自動検出サービスからの応答を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

自動検出要求と応答は、エンコードUTF-8必要があります。
  
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

