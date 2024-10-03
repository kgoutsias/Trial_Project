You find all endpoints for all cases below:

1. Ανάκτηση στοιχείων δικαιούχου.

http://localhost:8080/beneficiaries
http://localhost:8080/beneficiaries/1
1 is benef id

------------------------------------------------------

2. Ανάκτηση των λογαριασμών ενός δικαιούχου.

http://localhost:8080/accounts
http://localhost:8080/beneficiaries/1/accounts
1 is benef id

-------------------------------------------------------

3a. Ανάκτηση των συναλλαγών ana account.

http://localhost:8080/transactions
http://localhost:8080/beneficiaries/1/transactions
1 is acct id

-------------------------------------------------------

3b. Ανάκτηση των συναλλαγών ενός δικαιούχου.

http://localhost:8080/api/beneficiaries/1/transactions
1 is benef id

-------------------------------------------------------

4. Ανάκτηση του υπολοίπου των λογαριασμών ενός ανθρώπου.

http://localhost:8080/beneficiaries/1/balance

-------------------------------------------------------

5. Ανάκτηση της μεγαλύτερης ανάληψης για έναν δικαιούχο τον τελευταίο μήνα.

http://localhost:8080/api/608/largestWithdrawal
608 is benef id

{
    "transactionId": 25,
    "accountId": 227,
    "amount": 135.8,
    "type": "withdrawal",
    "date": "09/09/24"
}