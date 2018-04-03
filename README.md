# COMP6370-CyberSecurity
For Auburn University Software Engineering COMP 6370 Cyber Security

## UDP Needham-Schroeder Protocol
  Write a program that simulates the Needham-Schroeder protocol using Java, C, or C++.
  
  The program should consist of three actors:
  
    - Central authority (Cathy)
    - User 1 (Alice) 
    - User 2 (Bob)
The program should at least complete the forming of a session (initial nonce sent to CA, second nonce from user 2 and modified second nonce in reply from user 1), and they should at least exchange one message.

For each step of the simulation, show both the encrypted and unencrypted messages that are being sent, and indicate who is sending the message, and where it is being sent. 


For example, when Alice(A) is sending the session key to Bob(B):

Alice sending session key to Bob

Encrypted message is: *a;lskdjf;laksjdf;lkja*

Unencrypted message is: *This is Alice, Here is the Session Key* (of course it won’t really look like this)

### How to run the program

To run the program, please first compile the cpp file first. I used the g++ compiler on the school linux machines and compiled fine (with some warnings).

Then please run 3 different instances of the program, one to run Alice, Bob, and Cathy.

They can be ran either on the same machine, or different ones. 

Please run the program with Alice **LAST**, as Alice with be the actor to start of the messages, if she’s not started last the others will miss her initial request message!

If we compiled an a.out, 

To start up Bob and Cathy:

```
./a.out b

./a.out c
```
To start up Alice and watch the program run:

```
./a.out A [Cathy’s Host]  [Bob’s host]
```
  
Like this:
```
./a.out A tux062.eng.auburn.edu tux063.eng.auburn.edu
```
