---
title: メール、予定表、および連絡先の Office 365 REST API
manager: sethgros
ms.date: 4/29/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: メール、予定表、および連絡先にアクセスするのに使用できる Office 365 API に関する情報を Office 365 または Exchange Online で探します。
ms.openlocfilehash: d42d3ff0b68dfbf23d5a4eebb826a6d39a4ac116
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759175"
---
# <a name="office-365-rest-apis-for-mail-calendars-and-contacts"></a><span data-ttu-id="ed3b1-103">メール、予定表、および連絡先の Office 365 REST API</span><span class="sxs-lookup"><span data-stu-id="ed3b1-103">Office 365 REST APIs for mail, calendars, and contacts</span></span>

<span data-ttu-id="ed3b1-104">メール、予定表、および連絡先にアクセスするのに使用できる Office 365 API に関する情報を Office 365 または Exchange Online で探します。</span><span class="sxs-lookup"><span data-stu-id="ed3b1-104">Find information about the Office 365 APIs that you can use to access mail, calendars, and contacts in Office 365 or Exchange Online.</span></span>
  
<span data-ttu-id="ed3b1-p101">Office 365 および Exchange Online は、電子メール、予定表、および連絡先で作業する新しい方法を提供します。メール、予定表、および連絡先の REST API は、Exchange データへのアクセスと操作に関する強力で簡単な方法を提供します。これらの API は、オープン標準に基づいています:認証には OAuth バージョン 2.0、データ抽象化には OData バージョン 4.0 および JSON が該当します。これには以下の利点があります。</span><span class="sxs-lookup"><span data-stu-id="ed3b1-p101">Office 365 and Exchange Online provide a new way to work with email, calendars, and contacts. The Mail, Calendar, and Contact REST APIs provide a powerful, easy-to-use way to access and manipulate Exchange data. These APIs are based on open standards: OAuth version 2.0 for authentication, and OData version 4.0 and JSON for data abstraction. This provides the following advantages:</span></span>
  
- <span data-ttu-id="ed3b1-109">これらの API は認証に OAuth を求めるため、アプリケーションがユーザーの資格情報を処理または格納する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="ed3b1-109">Because these APIs require OAuth for authentication, your application does not have to handle or store user credentials.</span></span>
    
- <span data-ttu-id="ed3b1-p102">OAuth は、ユーザー データへの厳格に範囲指定されたアクセス許可を要求できるようにします。たとえば、アクセス許可を要求して、ユーザーの予定表のみを読み取るようにアプリケーションを設計する場合があります。</span><span class="sxs-lookup"><span data-stu-id="ed3b1-p102">OAuth makes it possible to request tightly scoped permissions to user data. For example, you might design your application to request permission and read only a user's calendar.</span></span>
    
## <a name="work-with-email-and-mail-folders"></a><span data-ttu-id="ed3b1-112">電子メールおよびメール フォルダーで作業する</span><span class="sxs-lookup"><span data-stu-id="ed3b1-112">Work with email and mail folders</span></span>

<span data-ttu-id="ed3b1-p103">[メール API](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx) を使用して、電子メールの取得、作成、更新、削除、移動、コピー、および送信を行うことができます。また、メール フォルダーの取得、作成、更新、および削除を行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="ed3b1-p103">You can use the [Mail API](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx) to get, create, update, delete, move, copy, and send email. You can also get, create, update, and delete mail folders.</span></span> 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a><span data-ttu-id="ed3b1-115">イベント、予定表、および予定表グループで作業する</span><span class="sxs-lookup"><span data-stu-id="ed3b1-115">Work with events, calendars, and calendar groups</span></span>

<span data-ttu-id="ed3b1-p104">[予定表 API](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx) を使用して、イベントの取得、作成、更新、および削除を行うことができます。また、予定表グループおよび予定表の取得、作成、更新、および削除を行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="ed3b1-p104">You can use the [Calendar API](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx) to get, create, update, and delete events. You can also get, create, update, and delete calendar groups and calendars.</span></span> 
  
## <a name="work-with-contacts-and-contact-folders"></a><span data-ttu-id="ed3b1-118">連絡先および連絡先フォルダーで作業する</span><span class="sxs-lookup"><span data-stu-id="ed3b1-118">Work with contacts and contact folders</span></span>

<span data-ttu-id="ed3b1-p105">[連絡先 API](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx) を使用して、ユーザーのメールボックス内の連絡先の取得、作成、更新、および削除を行うことができます。また、連絡先フォルダーの取得を行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="ed3b1-p105">You can use the [Contacts API](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx) to get, create, update, and delete contacts in a user's mailbox. You can also get contact folders.</span></span> 
  
## <a name="work-with-file-providers"></a><span data-ttu-id="ed3b1-121">ファイル プロバイダーの操作</span><span class="sxs-lookup"><span data-stu-id="ed3b1-121">Work with file providers</span></span>

<span data-ttu-id="ed3b1-122">[ファイル プロバイダーの REST API](http://msdn.microsoft.com/library/8bab5403-de68-4b49-ab19-9a6470f2a2ce%28Office.15%29.aspx) を使用して、メールボックス、Dropbox などのサポートされているファイル プロバイダーに関する情報を取得、作成、更新、削除することができます。</span><span class="sxs-lookup"><span data-stu-id="ed3b1-122">You can use the [File Providers REST API](http://msdn.microsoft.com/library/8bab5403-de68-4b49-ab19-9a6470f2a2ce%28Office.15%29.aspx) to get, create, update, and delete information about supported file providers, such as mailbox, Dropbox, and so on.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="ed3b1-123">次の手順</span><span class="sxs-lookup"><span data-stu-id="ed3b1-123">Next steps</span></span>

<span data-ttu-id="ed3b1-p106">[Office 365 プラットフォームでの開発](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx)ページに進んで、環境のセットアップおよび API を開始するためのガイダンスを含む、メール、予定表、および連絡先 API に関する情報を取得してください。また、[スタート プロジェクトおよびコード サンプル](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx)を必ず確認して、これらの API の動作を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed3b1-p106">Head over to the [Developing on the Office 365 platform](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx) page to get more information about the Mail, Calendar, and Contacts APIs, including guidance for setting up your environment and getting started with the APIs. Also be sure to check out the [starter projects and code samples](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx) to see these APIs in action.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ed3b1-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="ed3b1-126">See also</span></span>


- [<span data-ttu-id="ed3b1-127">Office 365 プラットフォーム上での開発</span><span class="sxs-lookup"><span data-stu-id="ed3b1-127">Developing on the Office 365 platform</span></span>](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx)
    
- [<span data-ttu-id="ed3b1-128">Office 365 ASP.NET MVC アプリの構築</span><span class="sxs-lookup"><span data-stu-id="ed3b1-128">Building an Office 365 ASP.NET MVC app</span></span>](http://msdn.microsoft.com/office/office365/howto/Build-your-first-ASPNET-MVC-app%28Office.15%29.aspx)
    
- [<span data-ttu-id="ed3b1-129">メール REST 操作</span><span class="sxs-lookup"><span data-stu-id="ed3b1-129">Mail REST operations</span></span>](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx)
    
- [<span data-ttu-id="ed3b1-130">予定表 REST 操作</span><span class="sxs-lookup"><span data-stu-id="ed3b1-130">Calendar REST operations</span></span>](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx)
    
- [<span data-ttu-id="ed3b1-131">連絡先 REST 操作</span><span class="sxs-lookup"><span data-stu-id="ed3b1-131">Contacts REST operations</span></span>](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx)
    
- [<span data-ttu-id="ed3b1-132">Office 365 API スタート プロジェクトおよびサンプル コード</span><span class="sxs-lookup"><span data-stu-id="ed3b1-132">Office 365 APIs starter projects and code samples</span></span>](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx)
    

