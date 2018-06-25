---
title: EncryptedSharedFolderDataCollection
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EncryptedSharedFolderDataCollection
api_type:
- schema
ms.assetid: 25c6ae87-bbb9-4dd5-a85a-d669fcea137f
description: EncryptedSharedFolderDataCollection 要素には、クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントとデータ構造体のコレクションが含まれています。
ms.openlocfilehash: e4d37f5df10f5e270be5126479485239f2205d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760273"
---
# <a name="encryptedsharedfolderdatacollection"></a>EncryptedSharedFolderDataCollection

**EncryptedSharedFolderDataCollection**要素には、クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントとデータ構造体のコレクションが含まれています。 
  
```xml
<EncryptedSharedFolderDataCollection>   <EncryptedSharedFolderData/></EncryptedSharedFolderDataCollection>
```

 **ArrayOfEncryptedSharedFolderDataType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[EncryptedSharedFolderData](encryptedsharedfolderdata.md) <br/> |クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントで暗号化されたデータが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |[GetSharingMetadata 操作](getsharingmetadata-operation.md)要求に対する応答を定義します。  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[GetSharingMetadata の操作](getsharingmetadata-operation.md)を要求します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetSharingMetadata 操作](getsharingmetadata-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

