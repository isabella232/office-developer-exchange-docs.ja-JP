---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: IconIndex 要素は、アイテムまたはスレッドのアイコンインデックスを識別します。
ms.openlocfilehash: 0f932f5632422a8786e74500bf83cb1337f780c3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460786"
---
# <a name="iconindex"></a><span data-ttu-id="84f30-103">IconIndex</span><span class="sxs-lookup"><span data-stu-id="84f30-103">IconIndex</span></span>

<span data-ttu-id="84f30-104">**IconIndex**要素は、アイテムまたはスレッドのアイコンインデックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="84f30-104">The **IconIndex** element identifies the icon index for an item or conversation.</span></span> 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MailIrmForwarded | MailIrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 <span data-ttu-id="84f30-105">**IconIndexType**</span><span class="sxs-lookup"><span data-stu-id="84f30-105">**IconIndexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="84f30-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="84f30-106">Attributes and elements</span></span>

<span data-ttu-id="84f30-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="84f30-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84f30-108">属性</span><span class="sxs-lookup"><span data-stu-id="84f30-108">Attributes</span></span>

<span data-ttu-id="84f30-109">なし。</span><span class="sxs-lookup"><span data-stu-id="84f30-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="84f30-110">子要素</span><span class="sxs-lookup"><span data-stu-id="84f30-110">Child elements</span></span>

<span data-ttu-id="84f30-111">なし。</span><span class="sxs-lookup"><span data-stu-id="84f30-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="84f30-112">親要素</span><span class="sxs-lookup"><span data-stu-id="84f30-112">Parent elements</span></span>

<span data-ttu-id="84f30-113">[会話 (ConversationType)](conversation-conversationtype.md)  | [アイテム](item.md)  | [連絡先](contact.md)  | [DistributionList](distributionlist.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [Calendaritem](calendaritem.md)  | [Postitem](postitem.md)  | [タスク](task.md)</span><span class="sxs-lookup"><span data-stu-id="84f30-113">[Conversation (ConversationType)](conversation-conversationtype.md) | [Item](item.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Message](message-ex15websvcsotherref.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="84f30-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="84f30-114">Text value</span></span>

<span data-ttu-id="84f30-115">次の表に、 **IconIndex**要素に使用できるテキスト値を示します。</span><span class="sxs-lookup"><span data-stu-id="84f30-115">The following table contains the possible text values for the **IconIndex** element.</span></span> 
  
|<span data-ttu-id="84f30-116">**値**</span><span class="sxs-lookup"><span data-stu-id="84f30-116">**Value**</span></span>|<span data-ttu-id="84f30-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="84f30-117">**Description**</span></span>|
|:-----|:-----|
|||
|<span data-ttu-id="84f30-118">既定</span><span class="sxs-lookup"><span data-stu-id="84f30-118">Default</span></span>  <br/> |<span data-ttu-id="84f30-119">既定のアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-119">Specifies the default icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-120">PostItem</span><span class="sxs-lookup"><span data-stu-id="84f30-120">PostItem</span></span>  <br/> |<span data-ttu-id="84f30-121">投稿アイテムのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-121">Specifies the icon for a post item.</span></span>  <br/> |
|<span data-ttu-id="84f30-122">MailRead</span><span class="sxs-lookup"><span data-stu-id="84f30-122">MailRead</span></span>  <br/> |<span data-ttu-id="84f30-123">[メールの閲覧] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-123">Specifies the mail read icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-124">メール未開封</span><span class="sxs-lookup"><span data-stu-id="84f30-124">MailUnread</span></span>  <br/> |<span data-ttu-id="84f30-125">[未読のメール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-125">Specifies the unread mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-126">メール返信</span><span class="sxs-lookup"><span data-stu-id="84f30-126">MailReplied</span></span>  <br/> |<span data-ttu-id="84f30-127">[返信済みメール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-127">Specifies the replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-128">メール転送</span><span class="sxs-lookup"><span data-stu-id="84f30-128">MailForwarded</span></span>  <br/> |<span data-ttu-id="84f30-129">[転送されたメール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-129">Specifies the forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-130">MailEncrypted</span><span class="sxs-lookup"><span data-stu-id="84f30-130">MailEncrypted</span></span>  <br/> |<span data-ttu-id="84f30-131">暗号化されたメールのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-131">Specifies the encrypted mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-132">MailSmimeSigned</span><span class="sxs-lookup"><span data-stu-id="84f30-132">MailSmimeSigned</span></span>  <br/> |<span data-ttu-id="84f30-133">[セキュリティで保護されたマルチパーパスインターネットメール内線 (S/MIME) 署名済みメール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-133">Specifies the Secure/Multipurpose Internet Mail Extensions (S/MIME) signed mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-134">MailEncryptedReplied</span><span class="sxs-lookup"><span data-stu-id="84f30-134">MailEncryptedReplied</span></span>  <br/> |<span data-ttu-id="84f30-135">[暗号化された返信メール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-135">Specifies the encrypted replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-136">MailSmimeSignedReplied</span><span class="sxs-lookup"><span data-stu-id="84f30-136">MailSmimeSignedReplied</span></span>  <br/> |<span data-ttu-id="84f30-137">S/MIME で署名された返信メールアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-137">Specifies the S/MIME signed replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-138">MailEncryptedForwarded</span><span class="sxs-lookup"><span data-stu-id="84f30-138">MailEncryptedForwarded</span></span>  <br/> |<span data-ttu-id="84f30-139">[暗号化された転送メール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-139">Specifies the encrypted forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-140">MailSmimeSignedForwarded</span><span class="sxs-lookup"><span data-stu-id="84f30-140">MailSmimeSignedForwarded</span></span>  <br/> |<span data-ttu-id="84f30-141">S/MIME で署名された転送メールアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-141">Specifies the S/MIME signed forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-142">MailEncryptedRead</span><span class="sxs-lookup"><span data-stu-id="84f30-142">MailEncryptedRead</span></span>  <br/> |<span data-ttu-id="84f30-143">[暗号化されたメールの開封] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-143">Specifies the encrypted read mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-144">MailSmimeSignedRead</span><span class="sxs-lookup"><span data-stu-id="84f30-144">MailSmimeSignedRead</span></span>  <br/> |<span data-ttu-id="84f30-145">S/MIME で署名されたメールの開封アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-145">Specifies the S/MIME signed read mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-146">MailIrm</span><span class="sxs-lookup"><span data-stu-id="84f30-146">MailIrm</span></span>  <br/> |<span data-ttu-id="84f30-147">Information Rights Management (IRM) で保護されたメールのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-147">Specifies the Information Rights Management (IRM)-protected mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-148">MailIrmForwarded</span><span class="sxs-lookup"><span data-stu-id="84f30-148">MailIrmForwarded</span></span>  <br/> |<span data-ttu-id="84f30-149">IRM で保護された転送されたメールのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-149">Specifies the IRM-protected forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-150">MailIrmReplied</span><span class="sxs-lookup"><span data-stu-id="84f30-150">MailIrmReplied</span></span>  <br/> |<span data-ttu-id="84f30-151">[IRM で保護された返信メール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-151">Specifies the IRM-protected replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-152">SmsSubmitted</span><span class="sxs-lookup"><span data-stu-id="84f30-152">SmsSubmitted</span></span>  <br/> |<span data-ttu-id="84f30-153">ショートメッセージサービス (SMS) ルーティングに送信されるメールのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-153">Specifies the icon mail submitted for Short Message Service (SMS) routing.</span></span>  <br/> |
|<span data-ttu-id="84f30-154">Smsルーブル Tedtodeliverypoint</span><span class="sxs-lookup"><span data-stu-id="84f30-154">SmsRoutedToDeliveryPoint</span></span>  <br/> |<span data-ttu-id="84f30-155">外部配信ポイントへの SMS ルーティングのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-155">Specifies the icon for SMS routing to an external delivery point.</span></span>  <br/> |
|<span data-ttu-id="84f30-156">Smsルーブル Tedtoexternalmessagingsystem</span><span class="sxs-lookup"><span data-stu-id="84f30-156">SmsRoutedToExternalMessagingSystem</span></span>  <br/> |<span data-ttu-id="84f30-157">外部メッセージングシステムへの SMS ルーティングのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-157">Specifies the icon for SMS routing to an external messaging system.</span></span>  <br/> |
|<span data-ttu-id="84f30-158">SmsDelivered</span><span class="sxs-lookup"><span data-stu-id="84f30-158">SmsDelivered</span></span>  <br/> |<span data-ttu-id="84f30-159">[SMS 配信メール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-159">Specifies the SMS delivered mail icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-160">OutlookDefaultForContacts</span><span class="sxs-lookup"><span data-stu-id="84f30-160">OutlookDefaultForContacts</span></span>  <br/> |<span data-ttu-id="84f30-161">連絡先の既定のアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-161">Specifies the default icon for contacts.</span></span>  <br/> |
|<span data-ttu-id="84f30-162">AppointmentItem</span><span class="sxs-lookup"><span data-stu-id="84f30-162">AppointmentItem</span></span>  <br/> |<span data-ttu-id="84f30-163">予定アイテムアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-163">Specifies the appointment item icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-164">AppointmentRecur</span><span class="sxs-lookup"><span data-stu-id="84f30-164">AppointmentRecur</span></span>  <br/> |<span data-ttu-id="84f30-165">定期的な予定のアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-165">Specifies the recurring appointment icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-166">AppointmentMeet</span><span class="sxs-lookup"><span data-stu-id="84f30-166">AppointmentMeet</span></span>  <br/> |<span data-ttu-id="84f30-167">会議アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-167">Specifies the meeting icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-168">AppointmentMeetRecur</span><span class="sxs-lookup"><span data-stu-id="84f30-168">AppointmentMeetRecur</span></span>  <br/> |<span data-ttu-id="84f30-169">[定期的な会議] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-169">Specifies the recurring meeting icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-170">AppointmentMeetNY</span><span class="sxs-lookup"><span data-stu-id="84f30-170">AppointmentMeetNY</span></span>  <br/> |<span data-ttu-id="84f30-171">会議への仮承諾応答のアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-171">Specifies the icon for a tentative response to the meeting.</span></span>  <br/> |
|<span data-ttu-id="84f30-172">AppointmentMeetYes</span><span class="sxs-lookup"><span data-stu-id="84f30-172">AppointmentMeetYes</span></span>  <br/> |<span data-ttu-id="84f30-173">[会議の承諾] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-173">Specifies the meeting acceptance icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-174">AppointmentMeetNo</span><span class="sxs-lookup"><span data-stu-id="84f30-174">AppointmentMeetNo</span></span>  <br/> |<span data-ttu-id="84f30-175">会議の辞退アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-175">Specifies the meeting declined icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-176">AppointmentMeetMaybe</span><span class="sxs-lookup"><span data-stu-id="84f30-176">AppointmentMeetMaybe</span></span>  <br/> |<span data-ttu-id="84f30-177">会議への応答の可能性があるアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-177">Specifies the icon for a maybe response to the meeting.</span></span>  <br/> |
|<span data-ttu-id="84f30-178">AppointmentMeetCancel</span><span class="sxs-lookup"><span data-stu-id="84f30-178">AppointmentMeetCancel</span></span>  <br/> |<span data-ttu-id="84f30-179">会議のキャンセルアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-179">Specifies the meeting cancel icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-180">AppointmentMeetInfo</span><span class="sxs-lookup"><span data-stu-id="84f30-180">AppointmentMeetInfo</span></span>  <br/> |<span data-ttu-id="84f30-181">[ミーティング情報] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-181">Specifies the meeting information icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-182">TaskItem</span><span class="sxs-lookup"><span data-stu-id="84f30-182">TaskItem</span></span>  <br/> |<span data-ttu-id="84f30-183">タスクアイテムアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-183">Specifies the task item icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-184">TaskRecur</span><span class="sxs-lookup"><span data-stu-id="84f30-184">TaskRecur</span></span>  <br/> |<span data-ttu-id="84f30-185">[定期タスク] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-185">Specifies the recurring task icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-186">TaskOwned 者</span><span class="sxs-lookup"><span data-stu-id="84f30-186">TaskOwned</span></span>  <br/> |<span data-ttu-id="84f30-187">タスクの所有者アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-187">Specifies the task owned icon.</span></span>  <br/> |
|<span data-ttu-id="84f30-188">TaskDelegated</span><span class="sxs-lookup"><span data-stu-id="84f30-188">TaskDelegated</span></span>  <br/> |<span data-ttu-id="84f30-189">タスクの委任アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="84f30-189">Specifies the task delegated icon.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="84f30-190">注釈</span><span class="sxs-lookup"><span data-stu-id="84f30-190">Remarks</span></span>

<span data-ttu-id="84f30-191">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="84f30-191">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="84f30-192">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="84f30-192">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="84f30-193">要素の情報</span><span class="sxs-lookup"><span data-stu-id="84f30-193">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84f30-194">Namespace</span><span class="sxs-lookup"><span data-stu-id="84f30-194">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="84f30-195">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="84f30-195">Schema name</span></span>  <br/> |<span data-ttu-id="84f30-196">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="84f30-196">Types schema</span></span>  <br/> |
|<span data-ttu-id="84f30-197">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="84f30-197">Validation file</span></span>  <br/> |<span data-ttu-id="84f30-198">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="84f30-198">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="84f30-199">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="84f30-199">Can be empty</span></span>  <br/> |<span data-ttu-id="84f30-200">false</span><span class="sxs-lookup"><span data-stu-id="84f30-200">false</span></span>  <br/> |
   

