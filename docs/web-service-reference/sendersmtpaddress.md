---
title: SenderSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderSmtpAddress
api_type:
- schema
ms.assetid: e39c7df7-4bfa-455f-b4bb-1f1d05398eec
description: SenderSmtpAddress 要素は、共有されるフォルダーを含むメールボックスに対応する SMTP 電子メール アドレスを表します。
ms.openlocfilehash: 70905dd1ae2c3df18224aceeea246b542d1338e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833334"
---
# <a name="sendersmtpaddress"></a>SenderSmtpAddress

**SenderSmtpAddress**要素は、共有されるフォルダーを含むメールボックスに対応する SMTP 電子メール アドレスを表します。 
  
```xml
<SenderSmtpAddress/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetSharingMetadata](getsharingmetadata.md) <br/> |共有への招待を識別する不透明な認証トークンを取得する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

SMTP アドレスを表す文字列値は、必要があります。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetSharingMetadata 操作](getsharingmetadata-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

