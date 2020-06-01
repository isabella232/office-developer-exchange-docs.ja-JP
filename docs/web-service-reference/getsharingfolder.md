---
title: GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: ed5bb61f-89c7-4baa-83ee-30f06a49ff9b
description: GetSharingFolder 要素は、指定された共有フォルダーのローカルフォルダー識別子を取得する要求を定義します。 これは、GetSharingFolder 操作の基本要素です。
ms.openlocfilehash: cb76c534d9b30d0a9d1b267396551eb2871e638a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460506"
---
# <a name="getsharingfolder"></a>GetSharingFolder

**Getsharingfolder**要素は、指定された共有フォルダーのローカルフォルダー識別子を取得する要求を定義します。 これは、 [Getsharingfolder 操作](getsharingfolder-operation.md)の基本要素です。
  
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
|[SmtpAddress](smtpaddress.md) <br/> |共有関係にある相手の SMTP 電子メールアドレスを表します。 この要素は必須です。  <br/> |
|[DataType](datatype.md) <br/> |共有フォルダーによって共有されるデータの種類を表します。 この要素は省略できます。  <br/> |
|[SharedFolderId](sharedfolderid.md) <br/> |ローカルフォルダーの識別子を取得する必要がある共有フォルダーの識別子を表します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

GetSharingFolder 要素には、 [Smtpaddress](smtpaddress.md)要素を含める必要があります。 GetSharingFolder 要素には、 [DataType](datatype.md)要素または[SharedFolderId](sharedfolderid.md)要素も含める必要がありますが、両方を含めることはできません。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetSharingFolder 操作](getsharingfolder-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

