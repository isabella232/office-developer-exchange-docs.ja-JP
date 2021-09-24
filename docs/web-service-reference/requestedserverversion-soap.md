---
title: RequestedServerVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: cf3f9d7a-2add-4457-b009-2929220f90b5
description: RequestedServerVersion 要素は、自動検出メソッドがターゲットを呼び出すサーバー バージョンを指定します。
ms.openlocfilehash: 0690481523ab48497c40338a8808dfa2ed9b0e99
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540560"
---
# <a name="requestedserverversion-soap"></a>RequestedServerVersion (SOAP)

**RequestedServerVersion** 要素は、自動検出メソッドがターゲットを呼び出すサーバー バージョンを指定します。 
  
```XML
<RequestedServerVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

**RequestedServerVersion** 要素のテキスト値は、自動検出メソッドがターゲットを呼び出すサーバー バージョンを指定します。 次の表に、有効なサーバー バージョンを示します。 
  
|**テキスト値**|**説明**|
|:-----|:-----|
|Exchange2007_SP1  <br/> |Exchange Server 2007 Service Pack 1 (SP1) を参照してください。  <br/> |
|Exchange2010  <br/> |Exchange Server 2010.  <br/> |
|Exchange2010_SP1  <br/> |Exchange Server 2010 Service Pack 1 (SP1) を参照してください。  <br/> |
|Exchange2010_SP2  <br/> |Exchange Server 2010 Service Pack 2 (SP2) を参照してください。  <br/> |
|Exchange2013  <br/> |Exchange Server 2013. Exchange2013 フィールドは、2013 年から 2013 年Exchange OnlineバージョンのクライアントExchange適用Exchange Serverです。  <br/> |
|Exchange2013_SP1  <br/> |Exchange Server 2013 Service Pack 1 (SP1) を参照してください。 [Exchange2013_SP1] フィールドは、2013 SP1 で始まる Exchange Onlineおよびバージョンの Exchangeを対象とするExchange Server適用されます。  <br/> |
   
## <a name="remarks"></a>注釈

**RequestedServerVersion** 要素は SOAP ヘッダーで設定されます。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空に設定可能  <br/> |はい  <br/> |
   

