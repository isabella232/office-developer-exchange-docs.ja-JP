---
title: EncryptedSharedFolderData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EncryptedSharedFolderData
api_type:
- schema
ms.assetid: c1d4ca18-c5ce-41ff-bab4-f75e358c8b9f
description: EncryptedSharedFolderData 要素には、クライアントが予定表の共有や他のクライアントとの連絡先データの共有を承認するために使用できる暗号化されたデータが含まれる。
ms.openlocfilehash: c86f615e8936a379f465afab337a264d27238537
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546624"
---
# <a name="encryptedsharedfolderdata"></a>EncryptedSharedFolderData

**EncryptedSharedFolderData** 要素には、クライアントが予定表の共有や他のクライアントとの連絡先データの共有を承認するために使用できる暗号化されたデータが含まれる。 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 **EncryptedSharedFolderDataType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[トークン](token.md) <br/> |共有データの識別トークンを表す暗号化されたデータが含まれます。  <br/> |
|[Data](data.md) <br/> |共有データを表す暗号化されたデータが含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[EncryptedSharedFolderDataCollection](encryptedsharedfolderdatacollection.md) <br/> |クライアントが予定表の共有または他のクライアントとの連絡先データの共有を承認するために使用できるデータ構造のコレクションを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetSharingMetadata 操作](getsharingmetadata-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

