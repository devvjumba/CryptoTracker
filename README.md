# CryptoTracker

This personal project looks to address the limitations of a popular cryptocurrency tracker so portfolios can be valued at any time.

Currently, I have only included Binance, one of the world's most popular crypto exchanges where many coins are traded every day. The greatest limitation I have found is once you withdraw your coins to sit in a cold storage wallet i.e. they are no longer on the exchange, it is impossible to track the value of your portfolio. Even on the exchange app itself, you only know the current value of your portfolio, and the workaround is to export your transaction history into 3 party apps to find profit/loss. This still doesn't allow you to see your cold storage amount.

This project works by using the exisiting exports to create a mass dataframe, whereby multiple exports can be fed in and give you a breakdown of your portfolio. It use's Binance's API to see real-time price movements. Even if part of your coins are in a cold wallet, this won't affect the valuation as they will have already been saved into the master table.

Next steps & opportunities for improvement:

My next action is to create plots that track your valuation over time. Seeing the entire portfolio, and also each coin, is feasible.

Currently, the import of the transaction history 'Export Transaction History {1}' is hard coded, whereby an easily copy-and-paste line subsitituing the number of the file is required. I think this could be further parameterised by using a 'for loop', but I haven't added it in yet.

The greatest limitation of this project it is locked into Binance only. Whilst having a large number of popular coins, it doesn't give all possible options, but will suffice for the majority of casual Crypto speculators, having access to 9/10 of the top ten coins by market share.
It is also hard coded to only use the two coins in my portfolio, this can be easily maniuplated in the comments written, but still is not as user-friendly and parameterised as I would like.

Because Binance requires a secret key (personal to you and should not be shared), the code itself won't work as I've removed my key. I've attached a table of the raw export, and the master dataframe to show the column names and allow the code to be followed regardless.
