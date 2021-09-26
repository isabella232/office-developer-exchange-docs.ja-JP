---
title: SharedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SharedFolderId
api_type:
- schema
ms.assetid: 21181ba3-9626-4284-9717-0b1c16948e8f
description: SharedFolderId 要素は、共有フォルダーの識別子を表し、GetSharingFolder 操作要求によって返されるローカル フォルダー識別子を表します。
ms.openlocfilehash: 7e47ba49abed99bdb3cfd00eb43d2ef276d4ef37
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545973"
---
# <a name="sharedfolderid"></a>SharedFolderId

**SharedFolderId 要素** は、共有フォルダーの識別子を表し [、GetSharingFolder](getsharingfolder-operation.md)操作要求によって返されるローカル フォルダー識別子を表します。 
  
```xml
<SharedFolderId/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetSharingFolder](getsharingfolder.md) <br/> |指定した共有フォルダーのローカル フォルダー識別子を取得する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、共有フォルダーの識別子を表す文字列で [、GetSharingFolder](getsharingfolder-operation.md) 操作要求によって返されるローカル フォルダー識別子です。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
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

