---
title: Exchange での EWS のアーカイブ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Exchange での EWS のアーカイブについて説明します。
ms.openlocfilehash: bc282a7774bb74e57550bc663512987839324b83
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758871"
---
# <a name="archiving-in-ews-in-exchange"></a>Exchange での EWS のアーカイブ

Exchange での EWS のアーカイブについて説明します。
  
アーカイブ メールボックスは、ユーザーに関連付けられている 2 番目のメールボックスです。通常、アーカイブ メールボックスはメールの格納域の制限に対処するために使用されます。たとえば、古いメール アイテムは、定期的に受信トレイからアーカイブ メールボックスに移動されます。  
  
Exchange Online、Office 365 の一部としての Exchange Online、および Exchange Server 2013 は、2 つの新しい Exchange Web サービス (EWS) 操作を導入し、これらを使用してプライマリ メールボックスからメール アイテムのセットをアーカイブできます。 この方法で受信トレイのアイテムをアーカイブすると、アイテムのフォルダー階層が保持されます。 さらに、アーカイブ メールボックスを、クライアント上にローカルに格納することもリモートで格納することもできるようなりました。その際、アーカイブのコンテンツを指すフォルダー パスを使用し、ユーザーにはほとんど見えない方法で行うことができます。
  
## <a name="archiving-operations-in-ews"></a>EWS でのアーカイブ操作

次の表に、Exchange 2013 で導入されたアーカイブ操作を記載します。 
  
|**操作名**|**説明**|
|:-----|:-----|
|[ArchiveItem](http://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |アイテムをプライマリ メールボックスからアーカイブ メールボックスに移動します。  <br/> |
|[CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |アーカイブ メールボックスの格納場所をポイントする URI を作成します。  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
    
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
    

