### Business Requirements

1. For each Client, work out who the most recent Account Manager is

The goal is to eliminate the duplicates that happened in the multiple Client ID and multiple Account Managers per Client. To start, split the RAW step into two Aggregate A) Aggregate for Client B) Aggregate for Training. A) is used to dedup the Client ID and Account Manager per Client(more on this later). B) is to make sure we have all the training info when we work on dedup.

One Client has multiple Account Manager and Client ID. The goal is to have keep the latest Account Manager per Client and Client ID. To do this we will need to create two Aggregate - 1) Client, Client, Account Manager and From Date 2) Client and From Date(set to Maximum). Join Aggregate 1) and 2) to eliminate the duplicates. 

2.Filter the data so that only the most recent Account Manager remains 

  a. Be careful not to lose any attendees from the training sessions!

3. In some instances, the Client ID has changed along with the Account Manager. Ensure only the most recent Client ID remains

Resource: https://community.tableau.com/s/question/0D54T00000C5Qy0SAF/use-tableau-prep-to-select-only-the-most-recent-record 
