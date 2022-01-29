# Bank simulation project

# Goal:

In this project, I am trying to build a software system that simulates a bank. There is one central bank that is connected to several ATMs and the bank receives and sends commands to these ATMs to perform transactions.

# Methodology:

The way I do that is to use pipes and concurrent processes. The simulator forks a number of processes that simulate a bank and a number of ATMs. Each ATM will read relevant information and send it to the bank using a pipe data structure. The bank receives commands from the ATMs, performs whatever transaction that the ATM command reads and then responds back to the ATM indicating a success or a failure in completing the transaction.
