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
description: UserConfigurationName 要素は、ユーザーの構成オブジェクトの名前を表します。 ユーザーの構成オブジェクトの名前は、ユーザーの構成オブジェクトの識別子です。
ms.openlocfilehash: 40580343e92493c3d39b090371708269ec3274b9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839924"
---
# <a name="userconfigurationname"></a>UserConfigurationName

**UserConfigurationName**要素は、ユーザーの構成オブジェクトの名前を表します。 ユーザーの構成オブジェクトの名前は、ユーザーの構成オブジェクトの識別子です。 
  
```XML
<UserConfigurationName Name="">
   <FolderId/>
</UserConfigurationName>
```

 **UserConfigurationNameType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**名前** <br/> |ユーザーの構成オブジェクトの名前を表す文字列値が含まれています。 この属性は、必要があります。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[フォルダー Id](folderid.md) <br/> |ユーザーの構成オブジェクトが含まれているフォルダーのフォルダー id を表します。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |ユーザーの構成オブジェクトが含まれているフォルダーの識別フォルダー名を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DeleteUserConfiguration](deleteuserconfiguration.md) <br/> |ユーザーの構成オブジェクトを削除する要求を表します。  <br/> |
|[GetUserConfiguration](getuserconfiguration.md) <br/> |ユーザーの構成オブジェクトを取得する要求を表します。  <br/> |
|[UserConfiguration](userconfiguration.md) <br/> |1 人のユーザーの構成オブジェクトを定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

