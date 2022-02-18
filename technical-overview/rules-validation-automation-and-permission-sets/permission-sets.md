# Permission Sets

Salesforce Permission Sets have been created to enable certain certain Users to do certain activities with the tool. This concept will also function to prevent users from accidentally deleting, editing or approving batches that they do not have permission to do.

There are 3 Permission Sets that have been created:&#x20;

1. **Edit\_Bulk\_Donation\_Template**&#x20;
   1. Admin users whom have been assigned to the `Edit_Bulk_Donation_Template` permission set can see the Settings button even if they don’t select a batch and close the first modal on page load stage + a toggle button is accessible for them in the Settings Modal to select which template they would like to update and see: Batch Level or Template Level: [Demo](https://take.ms/EEV9F).
   2. They are also able to update / edit templates on a Global scale, rather than it being Batch specific. Ie: Any changes they wish to make to a Template can be set for all Users using the tool compared to batch changes that only affect a specific batch.
   3. Should only be given to Administrators.
2. **Approve\_Bulk\_Donation**
   1. Those that should be able to _approve_ Batches that have been created and move Stages to Closed Won / Process CC Donations for created Opportunities.
3. **Delete\_Bulk\_Donation\_Template**&#x20;
   1. Vertic ADMIN only permission, should not be used by **any** users - acts to permit the deletion of Donation Templates completely.



