---
title: DataType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DataType
api_type:
- schema
ms.assetid: 267fe5aa-f9b1-4d4c-ac11-0f2e50ec2627
description: DataType 要素は、共有フォルダーで共有されるデータの種類を表します。
ms.openlocfilehash: 858165f32aebd523b10840246425c015353d659a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535857"
---
# <a name="datatype"></a>DataType

**DataType 要素** は、共有フォルダーで共有されるデータの種類を表します。 
  
```xml
<DataType>Calendar or Contacts</DataType>
```

**SharingDataType**

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

次の表に **、DataType** 要素に使用できる値を示します。 
  
**DataType 要素の値**

|**値**|**説明**|
|:-----|:-----|
|予定表  <br/> |共有フォルダーに予定表情報が含まれているかどうかを示します。  <br/> |
|連絡先  <br/> |共有フォルダーに連絡先情報が含まれているかどうかを示します。  <br/> |
   
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

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

