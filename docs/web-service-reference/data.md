---
title: データ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Data
api_type:
- schema
ms.assetid: f875e6c2-be18-439a-a7b1-bb49a149b538
description: Data 要素には、共有データを表す暗号化されたデータが含まれる。
ms.openlocfilehash: 1c28790467674e3ef44c9f0dc9e1fd706f880641
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535864"
---
# <a name="data"></a>データ

**Data 要素** には、共有データを表す暗号化されたデータが含まれる。 
  
- [EncryptedSharedFolderData](encryptedsharedfolderdata.md)  
- [Data](data.md)
  
```xml
<Data/>
```

**EncryptedDataContainerType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[EncryptedSharedFolderData](encryptedsharedfolderdata.md) <br/> |クライアントが予定表の共有または他のクライアントとの連絡先データの共有を承認するために使用できる暗号化されたデータを格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
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

