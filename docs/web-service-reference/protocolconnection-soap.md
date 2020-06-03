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
description: ProtocolConnection 要素は、サーバー Web クライアントのプロトコル接続を表します。
ms.openlocfilehash: b9df3febe36db53d7c5bf0610ba857f13aa96abc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528861"
---
# <a name="protocolconnection-soap"></a>ProtocolConnection (SOAP)

**Protocolconnection**要素は、サーバー Web クライアントのプロトコル接続を表します。 
  
```XML
<ProtocolConnection>
   <Hostname/>
   <Port/>
   <EncryptionMethod/>
</ProtocolConnection>
```

 **ProtocolConnection**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Hostname (SOAP)](hostname-soap.md) <br/> |コンピューターの完全なコンピューター名のホスト名部分を表します。  <br/> |
|[ポート (SOAP)](port-soap.md) <br/> |プロトコルに使用するポート番号を表します。  <br/> |
|[EncryptionMethod (SOAP)](encryptionmethod-soap.md) <br/> |POP、IMAP、および SMTP プロトコルに使用される暗号化方式を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ProtocolConnections (SOAP)](protocolconnections-soap.md) <br/> |0個以上のプロトコル接続を含みます。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[ProtocolConnectionCollectionSetting (SOAP)](protocolconnectioncollectionsetting-soap.md)

