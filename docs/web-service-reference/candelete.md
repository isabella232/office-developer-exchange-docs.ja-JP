---
title: CanDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CanDelete
api_type:
- schema
ms.assetid: 55e17121-aad0-4f90-889f-2c3512e9579c
description: CanDelete 要素は、管理フォルダーを顧客が削除できるかどうかを示します。
ms.openlocfilehash: ad7e573aeb2bb72d19f05421d0eab5a2f6ac5539
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516000"
---
# <a name="candelete"></a>CanDelete

**CanDelete** 要素は、管理フォルダーを顧客が削除できるかどうかを示します。 
  
```xml
<CanDelete/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |管理フォルダーに関する情報が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素が存在する場合は、ブール値を表すテキスト値が必要です。 値 true は **、** フォルダーを削除可能な状態を示します。false の **値は** 、フォルダーを削除できないことを意味します。 
  
## <a name="remarks"></a>注釈

管理フォルダーを削除するには [、DeleteFolder 操作を使用します](deletefolder-operation.md)。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateManagedFolder 操作](createmanagedfolder-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[フォルダーの削除](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

