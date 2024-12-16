# privilege-escalation-notes
1. REPORT LINK : https://www.netspi.com/blog/technical-blog/cloud-pentesting/escalating-privileges-in-google-cloud-via-open-groups/
     ### تلخيص

    1. **السيناريو المحتمل:**  
   - إذا كانت مجموعة Google (Google Group) تمتلك صلاحيات داخل Google Cloud (GCP).  
   - إعداد المجموعة يسمح لأي شخص في المؤسسة بالانضمام بدون موافقة.

    2. **الخطر:**  
   - أي موظف في المؤسسة يمكنه الانضمام إلى المجموعة المفتوحة ويرث صلاحياتها في GCP، مما يؤدي إلى **تصعيد الصلاحيات (Privilege Escalation)**.

    3. **السبب:**  
   - لا توجد قيود افتراضية تمنع المسؤولين من تخصيص صلاحيات لمجموعات مفتوحة الانضمام.

    4. **الإبلاغ:**  
   - تم اعتبار هذا السيناريو كخلل أمني محتمل وتم الإبلاغ عنه إلى Google.  
   - Google صنّفته كـ"تصرف مقصود" (Intended Behavior) ولن يتم إصلاحه.

    5. **الحل:**  
   - المسؤولون يجب أن يراجعوا إعدادات المجموعات ويتأكدوا من أن المجموعات الحساسة **ليست مفتوحة الانضمام** لأي شخص في المؤسسة.<br/>
  2. REPORT LINK :
     - Bypass Plan Restriction & Get 350$ Bounty : https://freedium.cfd/https://medium.com/@a13h1/bypass-plan-restriction-get-350-bounty-2df24f406462
  3. https://rhinosecuritylabs.com/research/vestaboard-vulnerabilities/ :
     - Read-Access to other Vestaboards. 
     - Ability to update names of other users. 
     - Privilege escalation from Admin to Owner.
  4. https://freedium.cfd/https://medium.com/h7w/how-i-earned-469-bounty-bypassing-plan-restriction-58f6d3120b6e
  5. https://cristivlad.medium.com/account-takeover-it-looked-secure-at-first-f14a31cb7f5c
  6. https://www.praetorian.com/blog/exploiting-broken-authentication-control-graphql/
  7. https://rashahacks.com/how-i-got-multiple-privilege-escalations/
  8. https://sayedv2.medium.com/how-i-discovered-authentication-bypass-that-blocks-users-from-accessing-the-website-93140fa180ac
  9. https://freedium.cfd/https://infosecwriteups.com/the-ui-slip-i-hit-750-ui-manipulation-leading-to-unauthorized-permission-changes-d65621d8dd96
