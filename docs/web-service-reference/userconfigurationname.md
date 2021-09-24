---
title: UserConfigurationName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserConfigurationName
api_type:
- schema
ms.assetid: 6947dd03-9727-4379-9b9d-42373fa120c7
description: UserConfigurationName 要素は、ユーザー構成オブジェクトの名前を表します。 ユーザー構成オブジェクト名は、ユーザー構成オブジェクトの識別子です。
ms.openlocfilehash: 7563435f25a5307aa908a64baceffb3c81138149
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517386"
---
# <a name="userconfigurationname"></a>UserConfigurationName

**UserConfigurationName** 要素は、ユーザー構成オブジェクトの名前を表します。 ユーザー構成オブジェクト名は、ユーザー構成オブジェクトの識別子です。 
  
```XML
<UserConfigurationName Name="">
   <FolderId/>
</UserConfigurationName>
```

```XML
<UserConfigurationName Name="">
   <DistinguishedFolderId/> 
</UserConfigurationName>
```

**UserConfigurationNameType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**名前** <br/> |ユーザー構成オブジェクトの名前を表す文字列値が含まれます。 この属性は必須です。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |ユーザー構成オブジェクトを含むフォルダーのフォルダー識別子を表します。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |ユーザー構成オブジェクトを含むフォルダーの識別フォルダー名を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DeleteUserConfiguration](deleteuserconfiguration.md) <br/> |ユーザー構成オブジェクトを削除する要求を表します。  <br/> |
|[GetUserConfiguration](getuserconfiguration.md) <br/> |ユーザー構成オブジェクトを取得する要求を表します。  <br/> |
|[UserConfiguration](userconfiguration.md) <br/> |1 つのユーザー構成オブジェクトを定義します。  <br/> |
   
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

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

