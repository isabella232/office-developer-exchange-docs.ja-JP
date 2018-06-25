---
title: EncryptedSharedFolderData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EncryptedSharedFolderData
api_type:
- schema
ms.assetid: c1d4ca18-c5ce-41ff-bab4-f75e358c8b9f
description: EncryptedSharedFolderData 要素には、クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントで暗号化されたデータが含まれています。
ms.openlocfilehash: 63966e95becaab4b3b1e54aa81f1b20a8b09dfd3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760275"
---
# <a name="encryptedsharedfolderdata"></a>EncryptedSharedFolderData

**EncryptedSharedFolderData**要素には、クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントで暗号化されたデータが含まれています。 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 **EncryptedSharedFolderDataType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[トークン](token.md) <br/> |共有データの識別トークンを表す暗号化されたデータが含まれています。  <br/> |
|[Data](data.md) <br/> |共有データを表す暗号化されたデータが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[EncryptedSharedFolderDataCollection](encryptedsharedfolderdatacollection.md) <br/> |クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントとデータ構造体のコレクションを表します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetSharingMetadata 操作](getsharingmetadata-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

