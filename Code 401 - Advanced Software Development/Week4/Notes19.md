July 6, 2023

Missed first hour
___________________________________________
  Prompt
Created class19 file only on local
Created shortcuts for making prompts

____________________________________________
  OS
import os

<!-- Make sure you are in your virtual env -->

os.mkdir('test_dir')
print('Directory Created')

<!-- Running (python3 filename.py) this will show file Exists -->

if os.path.exists('test_dir'):
  print('The directory already exists')
else:
  os.mkdir('test_dir')
  print('Directory Created')

<!-- This will create a folder if it does NOT exist. If it does exists, then it skips. -->

<!-- Create a new file -->
First things first
1. Where are we creating?
2. test_dir/test_file.txt
3. Create a file path

file_path = os.path.join('test_dir', 'test_file.txt')
print(f'Constructed File Path: {file_path})

with open(file_path, 'w') as file:
  file.write('Hello World!')

<!-- Refer to notes3 for more indepth explanation of 'with open' -->


os.mkdir
os.makedirs
What is the difference?
  Location
  
Mkdir assumes where you are at

Makedir can specify anywhere you are at, you need to tell it where it's going to exist.

mkdir exist_ok=True

folder 'src_directory'


hash:
Looks at all files on the backend. Gives you back a signature.










from rich.console import Console
from rich.prompt import Prompt
import sys
import os

def main():
  """Main function to run the CLI app."""
  console = Console()
  first = 'First'
  last = 'Last'
  while True:
    os.system('clear')
    console.print(f'\n1. First Name: {first}\n2. Last Name: {last}\n3. Full Name: {first} {last}\n4. Exit')
    choice = Prompt.ask('Choose a task (Enter the number)', choices=["1", "2", "3", "4"], default='4')
    
    if choice == '1':
      first = Prompt.ask('Please Enter your First Name:', default='First')
    elif choice == '2':
      last = Prompt.ask('Please Enter your Last Name:', default='Last')
    elif choice == '3':
      console.print(f'Your Full Name is: {first} {last}')
    elif choice == '4':
      do_exit('Thank you for using the menu')
    else:
      print('Try again')
      
def do_exit(message):
  sys.exit(message)
  
if __name__ == '__main__':
  try:
    main()
  except KeyboardInterrupt:
    do_exit('Ctrl-C detected. Exiting...')
__________________________________________

Regex101.com
This is how you will find out how to decipher.

sys 



___________________________________________
Labs

No starter tests

do 1-4 first THEN do 5

___________________________________________

Code Challenge 18

fizz buzz function
k-ary tree: two+ children