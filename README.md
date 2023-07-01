# Bitpac
Publicly auditable cooperatives that live on bitcoin

# What is a bitpac?

A bitpac is a cooperative whose members control some money and vote on how to spend it. It uses bitcoin multisig to enable group control and voting happens over nostr.

# So is this basically a DAO?

The short answer is yes. The long answer is no. Daos are supposed to be autonomous, which, at least to me, means humans do not control the decisions they make. Eth people have ruined the meaning of dao and turned it into "a smart conract where keyholders vote on how to spend some money." By that definition, yes, a bitpac is a dao. But to me, that's a perversion of the meaning. The only true dao would be a robot: a dao completely controlled by software. If actual *people* control the dao's money (through voting), then it's not a dao in my opinion, it's some kind of corporation -- in bitpac's case, a cooperative.

# Why did you make this?

One day I was looking up reasons why altcoins are stupid and I came across this gem: https://forum.sushi.com/t/establish-sushi-legal-defense-fund/11813

Basically there's an ethereum "dao" called sushiswap. They got sued by the SEC. In response they created a proposal to use the funds held by the voters in their "dao" to hire lawyers to defend themselves. The vote passed and the money went to a bunch of lawyers.

I thought that was pretty stupid, but I liked the voting part. Voting on expenditures doesn't make you a dao (in my opinion), but it's still pretty neat. So I made this tool so that bitcoiners can do something similar. Create a multisig by selecting people's profiles from nostr, pick a threshold of how many votes are needed to move the money, and the result you get is a public page where any keyholder can propose how they'd like to spend the money. Every voter gets to accept or reject that proposal, and voila! It's like what sushiswap did except on bitcoin.

# So this is nothing more and nothing less than a multisig. Why didn't you just call it a multisig? Why make a new name when "multisig" is fine?

A bitpac is a multisig with *public auditability.* Multisigs are usually private -- you normally don't disclose who's in them. With bitpac, you do. But if you just want to just call it a multisig that's fine with me. I still had fun making an interface for creating and managing multisigs, and I for one think this tool is unique enough that it merits a special name.

# Todo list

- [x] Make proposals disappear if enough keyholders reject them
- [x] Make proposals disappear if they aren't passed in a month
- [x] Disallow subdust outputs
- [x] If a user proposes spending the max amount or very close to it, don't create a change output
- [ ] Improve the user interface
- [ ] Let keyholders transfer or sell their voting rights
- [ ] Allow custom fees
- [ ] Automatically broadcast transactions
- [ ] Display a countdown on each proposal for when it disappears
- [ ] Add more items to this todo list

![](https://supertestnet.github.io/bitpac/bitpac.png)
