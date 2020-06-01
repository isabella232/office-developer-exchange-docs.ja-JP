---
title: UserConfigurationName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationName
api_type:
- schema
ms.assetid: 6947dd03-9727-4379-9b9d-42373fa120c7
description: UserConfigurationName 要素は、ユーザー構成オブジェクトの名前を表します。 ユーザー構成オブジェクトの名前は、ユーザー構成オブジェクトの識別子です。
ms.openlocfilehash: 020b55919f7f81602a5eb072652d82168607d306
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466032"
---
# <a name="userconfigurationname"></a>UserConfigurationName

**Userconfigurationname**要素は、ユーザー構成オブジェクトの名前を表します。 ユーザー構成オブジェクトの名前は、ユーザー構成オブジェクトの識別子です。 
  
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
|**名前** <br/> |ユーザー構成オブジェクトの名前を表す文字列型 (string) の値を格納します。 この属性は必須です。  <br/> |
   
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
|[UserConfiguration](userconfiguration.md) <br/> |1つのユーザー構成オブジェクトを定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

