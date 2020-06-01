---
title: Exchangeservice.requestedserverversion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: cf3f9d7a-2add-4457-b009-2929220f90b5
description: Exchangeservice.requestedserverversion 要素は、自動検出メソッドが呼び出し対象とするサーバーのバージョンを指定します。
ms.openlocfilehash: ff63c82943bdd3476a4284f5aa2075fc9c0194b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467908"
---
# <a name="requestedserverversion-soap"></a>Exchangeservice.requestedserverversion (SOAP)

**Exchangeservice.requestedserverversion**要素は、**自動検出**メソッドが呼び出し対象とするサーバーのバージョンを指定します。 
  
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

**Exchangeservice.requestedserverversion**要素のテキスト値は、**自動検出**メソッドが呼び出すサーバーのバージョンを指定します。 次の表に、有効なサーバーバージョンの一覧を示します。 
  
|**テキスト値**|**説明**|
|:-----|:-----|
|Exchange2007_SP1  <br/> |Exchange Server 2007 Service Pack 1 (SP1)。  <br/> |
|Exchange2010  <br/> |Exchange Server 2010。  <br/> |
|Exchange2010_SP1  <br/> |Exchange Server 2010 Service Pack 1 (SP1)。  <br/> |
|Exchange2010_SP2  <br/> |Exchange Server 2010 Service Pack 2 (SP2)。  <br/> |
|Exchange2013  <br/> |Exchange Server 2013。 Exchange2013 フィールドは、exchange Online と exchange Server 2013 以降のバージョンの Exchange を対象とするクライアントに適用されます。  <br/> |
|Exchange2013_SP1  <br/> |Exchange Server 2013 Service Pack 1 (SP1)。 Exchange2013_SP1 フィールドは、exchange Online と exchange Server 2013 SP1 以降のバージョンの Exchange を対象とするクライアントに適用されます。  <br/> |
   
## <a name="remarks"></a>注釈

**Exchangeservice.requestedserverversion**要素は、SOAP ヘッダーで設定されます。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |はい  <br/> |
   

