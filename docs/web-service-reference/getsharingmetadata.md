---
title: GetSharingMetadata
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: b609ee26-6d28-4559-81b6-b8e8d4759a23
description: GetSharingMetadata 要素は、共有の招待を識別する不透明な認証トークンを取得する要求を定義します。 この要素は、GetSharingMetadata 操作の基本要素です。
ms.openlocfilehash: 65da8371b25c42e59f898c79403f06fa17e5a24a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523054"
---
# <a name="getsharingmetadata"></a>GetSharingMetadata

**GetSharingMetadata** 要素は、共有の招待を識別する不透明な認証トークンを取得する要求を定義します。 この要素は [、GetSharingMetadata 操作の基本要素です](getsharingmetadata-operation.md)。
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 **GetSharingMetadataType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[IdOfFolderToShare](idoffoldertoshare.md) <br/> |共有するサーバー上のフォルダーの識別子を表します。 この要素は必須です。  <br/> |
|[SenderSmtpAddress](sendersmtpaddress.md) <br/> |[IdOfFolderToShare](idoffoldertoshare.md)要素によって識別されるフォルダーを含むメールボックスに対応する SMTP 電子メール アドレスを表します。 この要素は必須です。  <br/> |
|[Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |[IdOfFolderToShare](idoffoldertoshare.md)要素によって識別されるフォルダー内のデータへのアクセスを許可される 1 つ以上のエンティティの SMTP 電子メール アドレスを表します。 この要素は必須です。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetSharingMetadata 操作](getsharingmetadata-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

