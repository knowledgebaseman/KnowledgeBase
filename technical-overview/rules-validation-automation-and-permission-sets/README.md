---
description: Explanation of validation rules in place within the tool.
---

# Rules (Validation / Automation & Permission Sets)

**Approve** button is only available to those who carry the correct Permission Set (See Permission Sets Page). The action of the Approve Button will set the Stage of an Opportunity to Closed Won.

> Logic has been added to set the Stage Name Also, I have added logic to set the Stage Name to Closed Lost and Close Reason to the error message from the gateway if a CC transaction fails. When the table loads it checks the record for the Closed Lost stage as well and highlights the row in red.

* **Opportunity Amount vs Payment Amount (**[**Demo**](https://take.ms/OwJZH)**)**
* If Opp.Amount is blank, but Payment.Amount is not blank then it sets the Opp.Amount = Payment.Amount
* If Payment.Amount is blank, but Opp.Amount is not blank then it sets the Payment.Amount = Opp.Amount

When inputting a donors BSB, this will act to populate the Bank Name on the Payment Record using the Bank object: [Demo](https://take.ms/M6BC2)

The Amount & Payment Amount fields accept the following letters (Salesforce Native Functionality)

* e (e can identify 'e' numbers)
* k (when you type a number you can use the shortcut 'k' to automate the posting of a thousand. ie. 1K will translate to 1000 under Salesforce logic.
* m (m acts the same way, in terms of millions)
* b (b acts the same way, in terms of billions)
* t (t acts the same way, in terms of trillions)

{% hint style="info" %}
Note this logic is Salesforce logic as we are using native Amount fields, not within our control.
{% endhint %}

**Batch numbers have been added to the Batch Name:**

****![](<../../.gitbook/assets/image (6).png>)****

****

****

{% content-ref url="permission-sets.md" %}
[permission-sets.md](permission-sets.md)
{% endcontent-ref %}
