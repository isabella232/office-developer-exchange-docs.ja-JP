---
title: GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: ed5bb61f-89c7-4baa-83ee-30f06a49ff9b
description: GetSharingFolder 要素は、指定した共有フォルダーのローカル フォルダーの識別子を取得する要求を定義します。 それは、GetSharingFolder 操作の基本要素です。
ms.openlocfilehash: 7c2f31aa27c1cbde6cdad2b41a341916b4bed2ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831669"
---
# <a name="getsharingfolder"></a>GetSharingFolder

**GetSharingFolder**要素は、指定した共有フォルダーのローカル フォルダーの識別子を取得する要求を定義します。 それは、 [GetSharingFolder 操作](getsharingfolder-operation.md)の基本要素です。
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 **GetSharingFolderType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |共有の関係で相手の SMTP 電子メール アドレスを表します。 この要素は必須です。  <br/> |
|[DataType](datatype.md) <br/> |共有フォルダーが共有されているデータの種類について説明します。 この要素はオプションです。  <br/> |
|[SharedFolderId](sharedfolderid.md) <br/> |返される識別子を持つローカルのフォルダーの共有フォルダーの識別子を表します。 この要素はオプションです。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

GetSharingFolder 要素は、 [SmtpAddress](smtpaddress.md)要素を含める必要があります。 GetSharingFolder 要素は、[データ型](datatype.md)の要素または[SharedFolderId](sharedfolderid.md)要素では、いずれかも含まれている必要がありますが、両方を含めることはできません。 
  
この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetSharingFolder 操作](getsharingfolder-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

