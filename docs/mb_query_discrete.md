mb_query_discrete
-----------------
mb_query need whole bytes to work, if discrete in or outputs are going to be queried, that dosen't add up to whole bytes, the mb_query_discrete should be used.

```pascal
#mb_query.mb_addr := __MB_ADDR__;
#mb_query.mode := #mb_query.c.read.discrete_input;
#mb_query.data_addr := __DATA_ADDR__;
"mb_query_discrete"(data_ptr := array_of_seven_bools, 
                    mb_query := #mb_query);
```