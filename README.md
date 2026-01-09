<h1>EASY TO USE SUPERMARKET SIMULATOR</h1>
<p>
  It's a console app where user is asked for a amount of checkouts and items,
  or only ask for amount of checkouts and let items be randomized. 
  Each checkout is a DTO and a thread at the same time.

  The DTO part of the checkout, is becouse each one has data inside it, 
  in this case it has 2 properties, code (int) and item_amount (int).
  
  On the other hand, it's a thread too, not exactly, but let's break this down: 
  Checkout has a function that is the heart of how the simulation works, <bold>check_items()</bold>, 
  this function, as it's name say, check one by one each item asing to that checkout, as 
  mentioned before is a int variable, so it repeats a <bold>check_item()</bold> certain amount of times 
  before finishing, to simulate as it was checking items, it will wait from 1 to 3 sec to do each item, being 
  a random amount of time for each item.

  Last but not least, all threads are <bold>daemon</bold>, whenever the user wants to stop the simulation, it can be done 
  just by pressing 'Enter', once a checkout is done, is shown how many items it scanned and when all checkouts are done, 
  the program will exit
</p>
