# dndrolldice
"""
Program that controls rolls for DnD. Pick you die, pick your roll count,
add your multipliers and slay some monsters!
"""
from random import randint
from time import sleep

def roll_die_twenty():
    count = 0
    total = 0
    multipliers = input('Please choose a multiplier. If no multipliers exist then enter 1: ')
    addons = input('Please choose any other additives to your roll: ')
    while count < int(roll_count):
        roll = randint(1,20)
        total = roll + total
        count += 1
    final_count = int(total) * int(multipliers) + int(addons)
    print('You rolled: ' + str(final_count))
    if int(final_count) >= int(target_number):
        print("Success")
    else:
        print("Failure")
def roll_die_twelve():
    count = 0
    total = 0
    multipliers = input('Please choose a multiplier. If no multipliers exist then enter 1: ')
    addons = input('Please choose any other additives to your roll: ')
    while count < int(roll_count):
        roll = randint(1,12)
        total = roll + total
        count += 1
    if multipliers == 0:
        multipliers = 1
    else:
        final_count = int(total) * int(multipliers) + int(addons)
    print('You rolled: ' + str(final_count))
    if int(final_count) >= int(target_number):
        print("Success")
    else:
        print("Failure")
def roll_die_ten():
    count = 0
    total = 0
    multipliers = input('Please choose a multiplier. If no multipliers exist then enter 1: ')
    addons = input('Please choose any other additives to your roll: ')
    while count < int(roll_count):
        roll = randint(1,10)
        total = roll + total
        count += 1
    if multipliers == 0:
        multipliers = 1
    else:
        final_count = int(total) * int(multipliers) + int(addons)
    print('You rolled: ' + str(final_count))
    if int(final_count) >= int(target_number):
        print("Success")
    else:
        print("Failure")
def roll_die_eight():
    count = 0
    total = 0
    multipliers = input('Please choose a multiplier. If no multipliers exist then enter 1: ')
    addons = input('Please choose any other additives to your roll: ')
    while count < int(roll_count):
        roll = randint(1,8)
        total = roll + total
        count += 1
    if multipliers == 0:
        multipliers = 1
    else:
        final_count = int(total) * int(multipliers) + int(addons)
    print('You rolled: ' + str(final_count))
    if int(final_count) >= int(target_number):
        print("Success")
    else:
        print("Failure")
def roll_die_six():
    count = 0
    total = 0
    multipliers = input('Please choose a multiplier. If no multipliers exist then enter 1: ')
    addons = input('Please choose any other additives to your roll: ')
    while count < int(roll_count):
        roll = randint(1,6)
        total = roll + total
        count += 1
    if multipliers == 0:
        multipliers = 1
    else:
        final_count = int(total) * int(multipliers) + int(addons)
    print('You rolled: ' + str(final_count))
    if int(final_count) >= int(target_number):
        print("Success")
    else:
        print("Failure")
def roll_die_four():
    count = 0
    total = 0
    multipliers = input('Please choose a multiplier. If no multipliers exist then enter 1: ')
    addons = input('Please choose any other additives to your roll: ')
    while count < int(roll_count):
        roll = randint(1,4)
        total = roll + total
        count += 1
    if multipliers == 0:
        multipliers = 1
    else:
        final_count = int(total) * int(multipliers) + int(addons)
    print('You rolled: ' + str(final_count))
    if int(final_count) >= int(target_number):
        print("Success")
    else:
        print("Failure")
def roll_die_two():
    count = 0
    total = 0
    multipliers = input('Please choose a multiplier. If no multipliers exist then enter 1: ')
    addons = input('Please choose any other additives to your roll: ')
    while count < int(roll_count):
        roll = randint(1,2)
        total = roll + total
        count += 1
    if multipliers == 0:
        multipliers = 1
    else:
        final_count = int(total) * int(multipliers) + int(addons)
    print('You rolled: ' + str(final_count))
    if int(final_count) >= int(target_number):
        print("Success")
    else:
        print("Failure")

print('Welcome to the DnD dice roller')
print('Types of die: d2, d4, d6, d8, d10, d12, d20')
target_number = input('DM please choose the target number. If no target level then input 0: ')
die_side = input('Please choose what die you want: ')
roll_count = input('Please choose how many rolls you are going to do: ')
if die_side == 'd20':
    roll_die_twenty()
elif die_side == 'd12':
    roll_die_twelve()
elif die_side == 'd10':
    roll_die_ten()
elif die_side == 'd8':
    roll_die_eight()
elif die_side == 'd6':
    roll_die_six()
elif die_side == 'd4':
    roll_die_four()
elif die_side == 'd2':
    roll_die_two()
else:
    print('Please select a valid die')
    
