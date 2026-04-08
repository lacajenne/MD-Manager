
From Mathias

There are 8 standard SMBS roles part of SC1GOLD and INTCH will have 8 corresponding SMBS standard access packages for that. 
Chris Taylor is saying something specific about Compliance - I don't know about that. We have only those 8 and none of them are named something specifically for Compliance 
 
https://dev.azure.com/SimCorpCloud/Service%20Release%20Office/_wiki/wikis/Service-Release-Office/119968/INTCH-environments

	 
The SMBS roles are the ones prefixed with SC_SMBS
 
This is the first Excel we did, not part of the official documentation, but it's more compact - DO NOT DISTRIBUTE
https://simcorp.sharepoint.com/:x:/r/sites/ReleaseOffice/_layouts/15/Doc.aspx?sourcedoc=%7BD006D7B7-EB53-444A-A227-052DE405DE5A%7D&file=SC1%20auth%20roles%20and%20access%20packages%20-%20NEW.xlsx&action=default&mobileredirect=true
 
There are also client facing roles.  
A few of those are part of the standard, but they don't have access packages as clients are supposed to get those via some Azure sync called SCIM.
 
Any 'why' questions on authorization and roles are to be redirected to Mathias.


