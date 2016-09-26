##Database Design - September 26, 2016

#Transaction
+Date
+Type_ID
+Amount
+Account_ID
+Payee_IS
-Pending
-ID

#Account
+Name
-ID
-Description

#AccountBal
+AC_ID
+Date
-Amount

#Note
+Trans_ID
-NoteText

#TagToTrans
+Tag_ID
+Trans_ID

#Tags
+Name
+Description
-Tag_ID

#Type
+Name
+Description
-Type_ID

#Payee
+Name
+Description
-Payee_ID

#TagToPayee
+Tag_ID
+Trans_ID
