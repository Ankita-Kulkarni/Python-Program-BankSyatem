'''
NAME : Ankita Ajit Kulkarni
TITLE: Write a Python program that computes the net amount of a bank account based a transaction log from console input. The transaction log format is shown as following:
D 100 W 200 (Withdrawal is not allowed if balance is going negative. Write functions for withdraw and deposit) D means deposit while W means withdrawal.
Suppose the following input is supplied to the program:D 300, D 300 , W 200, D 100 Then, the output should be:500
'''


print("Welcome to Union Bank of India!")
i =input("\nEnter your account number ::")
balance = print("Balance amount :: 0")
print("\nEnter your choice:")
print("D :: Deposit")
print("W :: Withdrawal")
print("C :: Cancel Transaction")


def withdraw_amount(amount,balance):
	balance = balance - amount
	return balance
				
def deposit_amount(amount,balance):
	balance = balance + amount
	return balance
	
def bank_account():
	while True :
		n = input("\nWhat type of transaction you would like to do? ")
		
		for k in (n):
			
			global balance	
			if ( n == 'D'):
				amount = float(input("\nEnter amount to be Deposited :: "))
				q = input("Do you want to continue the transaction (Y : YeS)? ")
				if ( q == 'Y' ):
					balance = balance + amount
					print("Amount Deposited :: Rs",amount)
					print("Successfull Transaction!")
		
		
			if ( n == 'W'):
				amount = float(input("\nEnter amount to be Withdrawed :: "))
				p = input("Do you want to continue the transaction (Y : Yes)? ")
				if ( p == 'Y' ):
					if (balance > amount):
						balance = balance - amount
						print("You Withdrawed :: Rs",amount)
						print("Successfull Transaction!")
					else:
						print("Insufficient Balance")
				else:
					print("Transaction Cancelled!")
			print("\t\t\t\t\t\t\t\tNet balance :: Rs {}".format(balance))	
			
		if ( n == 'C'):
			print("Transaction Cancelled!")
			
			break	

balance = 0
bank_account()
