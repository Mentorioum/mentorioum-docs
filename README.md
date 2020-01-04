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
- If `User` types `Rejected`, then `Bot` removes previously created repository and close the task   
1. `Bot`  closes task and creates next issue in `c101-basic-react-<userlogin>` repository according to cource agenda.

