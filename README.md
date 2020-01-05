# mentorioum-docs

Mentorium Docs

Drawing initial idea for Mentorium ecosystem, start with readme then organize content by the way

Use Cases:

# Rollup

1. `User` goes to 'mentorium-issues' and creates issue 'Rollup to Mentorium Course' 
1. `Bot` sends next message `We have next cources to rollup: #c101. Basic React #c101. Advanced React etc. Choose cource your want by typing cource id or description.`
1.  `User` sends message `#c101`  
1.  `Bot`  sends messsage `We have rolled up <userlogin> to cource. Repository for the cource created at 'c101-basic-react-<userlogin>'. Please check that repository was created. If everything is ok, then type 'Confirm', otherwise type 'Reject'`
1. `User` types `Confirm`
    1. If `User` types `Rejected`, then `Bot` removes previously created repository and close the task   
1. `Bot`  sends message: 
    1. If `User` have configured `Wallet` then message is:  `I've created 'c101-basic-react-<userlogin>' repository. And first task for you 'here'.`
    1. If `User` haven't configured `Wallet`them message is : `I've created 'c101-basic-react-<userlogin>' repository. And first task for you 'here'. HOWHEWERE you don't have configured 'Wallet', so we can't assign human participant for your. It means that you wont't able to make a 'help-me tikets'  and loose 'Score' because you won't have code reviews for your excercices. Do you wan't to configure 'Wallet' ? (Yes/No)`
1. `User` types
    1. If `User` types `Yes`, then `Bot` creates new task `Configure Wallet <userlogin>` and sends next message: `Created tasks 'here' for configring 'Wallet'. Closing this task.`
    1. If `User` types `No`, then `Bot` sends message `Hmm, ok. Closing task as far as rollup done`. `Bot` closes task.
    
  
