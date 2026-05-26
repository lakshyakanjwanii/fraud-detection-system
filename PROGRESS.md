Day 1: Environment setup
Day 2: Types of Frauds:
    Card Not Present -  card is not physically present on the scammer and the card details have been copied. Can be prevented by spending analysis and biometric scan.

    Account Takeover - scammer logs into the account and logs the user out and steals all the data. Can be prevented by 2FA via biometrics and password change to log scammer out of all accounts.

    Velocity Abuse - scammer makes multiple transactions in a short time duration to check usability of card. Can be prevented by monitoring spending analysis and ip address tracking and location tracking.

    Synthetic Identity - scammer makes a completely new personality by mixing parts of a person's real details and also fake details so scam cannot be traced back to a singular person. Can be prevented by behaviour analysis and biometric checking.
Day 3: 
    3.5% fraud rate

    Fraud average amount only 3% higher than legitimate

    Top missing columns at 90%+

    Dataset contains transaction id and value of how likely it is an fraudulent transaction on a scale of 0 to 1 and also contains time of transaction, amount and device through which transaction took place.

    The fraud rate of the dataset is 3.5% vs the real world transactions have a fraud rate of 0.1%. higher fraud rate in dataset helps model learn and flag transactions efficiently.

    Transaction amounts are not a good measure to verify whether a transaction is fraudulent or not.

    Time pattern chart showed us that most transactions take place during hours 17 to 24 and the number or transaction increase/decrease is proportional to number of fraud transactions. also the most fraud transactions take place during hours 0 and 1 due to automated fraud scripts.

    I merged both files using left join as to not miss any transactions and also to join related data to a transaction if it exists.
Day 4: 
    Understood data and its structure
Day 5: 
    Started with 435 columns, dropped 208 high missing value columns
    Filled numerical missing values with median
    Filled categorical missing values with Unknown
    Label encoded 13 categorical columns
    Scaled all numerical columns with StandardScaler
    Saved cleaned dataset to data/processed/cleaned_data.csv

       
