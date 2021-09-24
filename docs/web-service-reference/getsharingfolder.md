---
title: GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: ed5bb61f-89c7-4baa-83ee-30f06a49ff9b
description: GetSharingFolder 要素は、指定した共有フォルダーのローカル フォルダー識別子を取得する要求を定義します。 GetSharingFolder 操作の基本要素です。
ms.openlocfilehash: 5d6362dff3ff29b0dc5100780cc70b21ec9bee9d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509771"
---
# <a name="getsharingfolder"></a>GetSharingFolder

**GetSharingFolder** 要素は、指定した共有フォルダーのローカル フォルダー識別子を取得する要求を定義します。 [GetSharingFolder 操作の基本要素です](getsharingfolder-operation.md)。
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 **GetSharingFolderType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |共有関係の相手の SMTP 電子メール アドレスを表します。 この要素は必須です。  <br/> |
|[DataType](datatype.md) <br/> |共有フォルダーで共有されるデータの種類について説明します。 この要素は省略できます。  <br/> |
|[SharedFolderId](sharedfolderid.md) <br/> |ローカル フォルダー識別子を返す必要がある共有フォルダーの識別子を表します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

GetSharingFolder 要素には [、SmtpAddress 要素が含まれている必要](smtpaddress.md) があります。 GetSharingFolder 要素には [、DataType](datatype.md) 要素または [SharedFolderId](sharedfolderid.md) 要素のいずれかを含め、両方を含めません。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetSharingFolder 操作](getsharingfolder-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

