---
title: RequestedServerVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: cf3f9d7a-2add-4457-b009-2929220f90b5
description: RequestedServerVersion 要素は、サーバーのバージョンが、自動検出の方法でターゲットを呼び出すことを指定します。
ms.openlocfilehash: 6b9d31f3b7bca087652f04e4943becc5ac4e68e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833132"
---
# <a name="requestedserverversion-soap"></a>RequestedServerVersion (SOAP)

**RequestedServerVersion**要素は、サーバーのバージョンが、**自動検出**の方法でターゲットを呼び出すことを指定します。 
  
```XML
<RequestedServerVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

**RequestedServerVersion**要素のテキスト値は、サーバーのバージョンが、**自動検出**の方法でターゲットを呼び出すことを指定します。 次の表は、有効なサーバーのバージョンを示します。 
  
|**テキスト値**|**説明**|
|:-----|:-----|
|Exchange2007_SP1  <br/> |2007 Service Pack 1 (SP1) を Exchange Server です。  <br/> |
|Exchange2010  <br/> |Exchange Server 2010。  <br/> |
|Exchange2010_SP1  <br/> |2010 Service Pack 1 (SP1) を Exchange Server です。  <br/> |
|Exchange2010_SP2  <br/> |2010 Service Pack 2 (SP2) を Exchange Server です。  <br/> |
|Exchange2013  <br/> |Exchange Server 2013。 Exchange2013 フィールドは、Exchange Online とのバージョンの Exchange が Exchange Server 2013 以降を対象とするクライアントに適用されます。  <br/> |
|Exchange2013_SP1  <br/> |2013 Service Pack 1 (SP1) を Exchange Server です。 Exchange2013_SP1 フィールドは、オンラインの Exchange および Exchange が Exchange Server 2013 sp1 以降のバージョンを対象とするクライアントに適用されます。  <br/> |
   
## <a name="remarks"></a>備考

**RequestedServerVersion**要素は、SOAP ヘッダーで設定されています。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   

