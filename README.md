# faucet

THIS IS A PLACEHOLDER FOR NOW

Just thinking out loud here about one possible route

We're going to need one, possibly sooner rather than later. 
My initial thoughts are that this may be a good way to distribute test coins amongst the testnetters should we implement Pay to Upload as a method to throttle uploads in the short term.

Initialise a network and its associated genesis DBC
Create a tauri/yew form that asks for :-
 + forum handle
 + wallet address
 + public key
 + add a checkbox to agree to simple rules (discuss)  acknowledgement these are zero fiat-value testcoins etc
 + add a "Send me coins" button

For now store this in a simple Posacknowledgetgres/MariaDB/SQLite on the faucet admins PC <-crude but hopefully effective, this is just to do an "internal" job for now. We will eat our own dogfood as soon as it is proven fit for purpose. Lessons learnt will inform the eventual public-facing faucet. Which will most likely be a Maidsafe company responsibility anyway

Send a tiny amount of SNT to each participant - we want to conserve the vast majority of SNT for other testing.
Get the devs to implement a rule on uploads such that each Mb uploaded must be accompanied with a payment of n SNT where n is very small but non-zero. Details to be thrashed out as we go.
