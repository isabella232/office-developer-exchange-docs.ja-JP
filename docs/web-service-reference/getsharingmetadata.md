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
description: GetSharingMetadata 要素は、共有への招待を識別する不透明な認証トークンを取得する要求を定義します。 この要素は、GetSharingMetadata 操作の基本要素です。
ms.openlocfilehash: 5283d35e11350ef10ed8cc01527e787ef54be927
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831677"
---
# <a name="getsharingmetadata"></a>GetSharingMetadata

**GetSharingMetadata**要素は、共有への招待を識別する不透明な認証トークンを取得する要求を定義します。 この要素は、 [GetSharingMetadata 操作](getsharingmetadata-operation.md)の基本要素です。
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 **GetSharingMetadataType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[IdOfFolderToShare](idoffoldertoshare.md) <br/> |共有されるサーバー上のフォルダーの識別子を表します。 この要素は必須です。  <br/> |
|[SenderSmtpAddress](sendersmtpaddress.md) <br/> |[IdOfFolderToShare](idoffoldertoshare.md)要素で指定されているフォルダーを含むメールボックスに対応する SMTP 電子メール アドレスを表します。 この要素は必須です。  <br/> |
|[受信者 (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |[IdOfFolderToShare](idoffoldertoshare.md)要素で指定されたフォルダー内のデータへのアクセスを許可する 1 つまたは複数のエンティティの SMTP 電子メール アドレスを表します。 この要素は必須です。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetSharingMetadata 操作](getsharingmetadata-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

