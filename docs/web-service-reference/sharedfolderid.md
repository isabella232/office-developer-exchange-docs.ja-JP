---
title: SharedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharedFolderId
api_type:
- schema
ms.assetid: 21181ba3-9626-4284-9717-0b1c16948e8f
description: SharedFolderId 要素は、GetSharingFolder 操作要求によって返される必要のあるローカルフォルダー識別子である、共有フォルダーの識別子を表します。
ms.openlocfilehash: 546e148540708725bcf335f39bf69d193124d210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466123"
---
# <a name="sharedfolderid"></a>SharedFolderId

**SharedFolderId**要素は、 [getsharingfolder 操作](getsharingfolder-operation.md)要求によって返される必要のあるローカルフォルダー識別子である、共有フォルダーの識別子を表します。 
  
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
|[GetSharingFolder](getsharingfolder.md) <br/> |指定された共有フォルダーのローカルフォルダー識別子を取得する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、 [Getsharingfolder 操作](getsharingfolder-operation.md)要求によって返されるローカルフォルダー識別子である、共有フォルダーの識別子を表す文字列です。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
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

