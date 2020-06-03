---
title: GetSharingMetadata
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: b609ee26-6d28-4559-81b6-b8e8d4759a23
description: GetSharingMetadata 要素は、共有への招待を識別する非透過の認証トークンを取得する要求を定義します。 この要素は、GetSharingMetadata 操作の基本要素です。
ms.openlocfilehash: 406908e566d6d4249003b1a19a9ce79b8b328c4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530847"
---
# <a name="getsharingmetadata"></a>GetSharingMetadata

**Getsharingmetadata**要素は、共有への招待を識別する非透過の認証トークンを取得する要求を定義します。 この要素は、 [Getsharingmetadata 操作](getsharingmetadata-operation.md)の基本要素です。
  
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
|[IdOfFolderToShare](idoffoldertoshare.md) <br/> |共有されるサーバー上のフォルダーの識別子を表します。 この要素は必須です。  <br/> |
|[SenderSmtpAddress](sendersmtpaddress.md) <br/> |[IdOfFolderToShare](idoffoldertoshare.md)要素によって識別されるフォルダーが含まれているメールボックスに対応する SMTP 電子メールアドレスを表します。 この要素は必須です。  <br/> |
|[受信者 (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |[IdOfFolderToShare](idoffoldertoshare.md)要素によって識別されるフォルダー内のデータへのアクセスが許可される1つ以上のエンティティの SMTP 電子メールアドレスを表します。 この要素は必須です。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetSharingMetadata 操作](getsharingmetadata-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

