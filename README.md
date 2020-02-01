# q-2
debug 2.04
star 
declarations
  string name
  num quantity
  num PRICE_EACH = 2.00
  num total
  string PROMPT 1 = "Enter name"
  string PROMPT 2 = " Enter quantity"
  string QUIT = "XXX"
  string END_MSG = "END of job"
housekeeping()
  output PROMPT 1
  input name
return
quit
  detailloop()
    output PROMPT 2
    input quantity
    total = quantity * PRICE_EACH
    output name, total
    output PROMPT 1
  return
  quit
  endOfJob()
    output END_MSG
    stop
