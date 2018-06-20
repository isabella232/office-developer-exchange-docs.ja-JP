---
title: ProtocolConnection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6eef2188-6194-48f1-ad7e-46104aecdf56
description: ProtocolConnection 要素は、サーバーの Web クライアントのプロトコルの接続を表します。
ms.openlocfilehash: 8b5396821cd959e41d24fcf7a94c519f9c634a1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832915"
---
# <a name="protocolconnection-soap"></a>ProtocolConnection (SOAP)

**ProtocolConnection**要素は、サーバーの Web クライアントのプロトコルの接続を表します。 
  
```XML
<ProtocolConnection>
   <Hostname/>
   <Port/>
   <EncryptionMethod/>
</ProtocolConnection>
```

 **ProtocolConnection**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ホスト名 (SOAP)](hostname-soap.md) <br/> |コンピューターのフル コンピューター名のホスト名の部分を表します。  <br/> |
|[ポート (SOAP)](port-soap.md) <br/> |プロトコルに使用するポート番号を表します。  <br/> |
|[EncryptionMethod (SOAP)](encryptionmethod-soap.md) <br/> |POP、IMAP、および SMTP のプロトコルに使用される暗号化メソッドを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ProtocolConnections (SOAP)](protocolconnections-soap.md) <br/> |0 個以上のプロトコルの接続が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[ProtocolConnectionCollectionSetting (SOAP)](protocolconnectioncollectionsetting-soap.md)

