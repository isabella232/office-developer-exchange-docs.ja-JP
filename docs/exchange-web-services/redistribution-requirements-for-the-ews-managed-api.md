---
title: EWS マネージ API の再配布の要件
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: EWS マネージ API アセンブリをアプリケーションと共に再配布する方法を紹介します。
ms.openlocfilehash: f43156838c735cfc17106deb7860329d3da6c07a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531331"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a>EWS マネージ API の再配布の要件

EWS マネージ API アセンブリをアプリケーションと共に再配布する方法を紹介します。
  
EWS マネージ API アプリケーションを設計する際には、ユーザーにリリースする方法も検討してください。 
  
## <a name="redistributing-your-ews-managed-api-application"></a>EWS マネージ API アプリケーションの再配布

アプリケーションが Exchange サーバー上に配置されている場合を除き、EWS マネージ API アセンブリを再配布する必要があります。EWS マネージ API のダウンロードには、再配布できる次の 2 つのアセンブリが含まれています。Microsoft.Exchange.WebServices.dll と Microsoft.Exchange.WebServices.Auth.dll。EWS マネージ API アプリケーションをリリースする方法を設計する際に、次の情報を考慮してください。
  
- EWS マネージ API は、ダウンロードして、Exchange サーバーを対象とするアプリケーションと共に配布できるように設計されています。また、アプリケーションで EWS マネージ API をダウンロードすることもできます。
    
- EWS マネージ API を使用して、Exchange Online、Office 365 の一部としての Exchange Online、または Exchange Server 2007 以降のオンプレミス バージョンの Exchange と通信することができます。
    
- バージョン 2.1 以降のバージョンの EWS マネージ API で、グローバル アセンブリ キャッシュ (GAC) に API をインストールできます。MSI は自動的に DLL を GAC に追加し、ユーザーごとではなく、コンピューターごとにアクセス可能である。
    
ライセンス条項は EWS マネージ API のダウンロードに含まれています。EWS マネージ API で実行できる作業に関する認証情報の条項について確認してください。
  
## <a name="see-also"></a>関連項目


- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
    
- [EWS マネージ API (ダウンロード)](https://aka.ms/ews-managed-api-readme)
    

