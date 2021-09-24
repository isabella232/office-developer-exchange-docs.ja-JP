---
title: SharingEffectiveRights (PermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: 808bb4a1-aa2d-48c5-94b3-551b52c348bd
description: SharingEffectiveRights 要素は、共有されている連絡先データに対してユーザーが持つアクセス許可を示します。
ms.openlocfilehash: ecae44dd99f61e1e59648134d10190a758a28b17
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531780"
---
# <a name="sharingeffectiverights-permissionreadaccesstype"></a>SharingEffectiveRights (PermissionReadAccessType)

**SharingEffectiveRights** 要素は、共有されている連絡先データに対してユーザーが持つアクセス許可を示します。 
  
```XML
<SharingEffectiveRights>None | FullDetails</SharingEffectiveRights >
```

 **PermissionReadAccessType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ContactsFolder](contactsfolder.md) <br/> |メールボックスに含まれる連絡先フォルダーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、SharingEffectiveRights 要素で使用できる値を示** します。 
  
**SharingEffectiveRights 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |ユーザーがフォルダー内のアイテムを読み取るアクセス許可を持たなかどうかを示します。  <br/> |
|FullDetails  <br/> |ユーザーがフォルダー内のすべてのアイテムを読み取るアクセス許可を持っているかどうかを示します。  <br/> |
   
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



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

