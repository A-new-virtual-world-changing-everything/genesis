# genesis
architecture design of the whole world
this repos is only meant for ideas/design/architecture


##roles


* human

* supervised robot

* robot

* message


##principles

* every msg flowing through has got cost and credit to win

##ideas

human cm would like to ask a question: what is today's weather? he likes to pay $10 to get the result

```

msg:
    type: question
    reward: $10
    expires: 24hrs
    question: 
        what is the weather like today?

human/company need to :
    own a identity or 
    a supervised robot or
    a full automated robot to
        action: send the message to the vw's routing bus

initial context:
    human's ID has got initial assest of 0
    if an ID's assest is + means he has value, the greater the assest, greater the credit of the ID

rules:
    a human/company <-> ID, he can exchange the assest with real world money


txn:
    a txn is a message's requested payload is completed by human/company's representitive, eg himself or the robot
    the requester is happy with the result and agree to pay for the promised reward

profit:
    a txn's reward - all cost during the routing: (vw network routing degrading cost + midman charges + bank/financial charges + deliver fee + whatever mid man/proc fee)= final profit


roles:
    whether you are a human/robot/supervised robot or a org/company, you will have a role associate with  it
    eg:
        it can be a broker : make a living for processing received msg or discoverable msg, process and deliver the requested result
        or can be a vw bank: lend money or charge interest
        or a insurer: gurantee the service or service charge will be paid and temporily hold the deposit

#system

msg routing:
    when msg is shot out, it is replicated to a few peer to peer nodes or a centralised for further routing
    msg could be privately dispatched to friends, known brokers as first priority, then vw network
    a ID could either receive a msg directly from another ID, or discover the relevant msgs from wv network

msg store:
    msg tends to scatter distributed but not centralised. 

vw server:
    idealy, there shouldn't be a central server to serve as brain or stroage

msg payload:
   msg payload type: 
        static informational message no brain stuff
        runable code containing solution/logic with brain

vw distributed code exec server:
    ideally be provided by an ID role of ISP earning credit for its service

security:
    each msg's senstive part will be encrypted to BASE64 using pki to be carried over during routing

```

##virtual world universal message structure

<div align="center">
<img alt="vw-umsg" 
src="https://raw.githubusercontent.com/A-new-virtual-world-changing-everything/genesis/master/design/vw_umsg.png" />
</div>
