```mermaid
flowchart TB
    subgraph before
       
        CS101
        CS149
        %% one --> two
        %% CS149 --> CS159
   
        CS159
        CS227
 
    end
 
    subgraph after
    %% two --> three
    subgraph three
        subgraph three_one
            CS261
            CS240
        end
        CS345
    end
   
    subgraph Elective
        subgraph permission
            CS280
            CS497
            CS499
        end
        CS374
        CS343
        CS347
        CS330
        CS354
        CS444
        CS445
        CS488
        CS442
        CS447
       
        
        subgraph NSA
            CS457
        CS458
        CS482
        end
       
        
    end
    %%two <--> Elective
    %% three --> four
    subgraph four
        subgraph four_one
            CS361
            CS327
        end
       
        subgraph Algorithm
            CS412
            CS452
        end
        subgraph System
            CS432
            CS450
            CS456
            CS470
            CS455
        end
       
        CS430
       
    end
        %% connections
        %%first
        CS149 --> CS159
        %%second
        CS159 --> CS261
        CS159 --> CS240
        CS159 --> CS345
        CS159 --> CS261
        %% CS227 --> CS327
        CS227 --> CS240
        %%thrid
        CS261 --> CS361
        CS261 --> CS430
        CS261 --> CS488
        CS261 --> CS482
        CS240 --> CS327
        CS240 --> CS412
        CS240 --> CS452
        CS240 --> CS354
        CS240 --> CS361
        CS240 --> CS430
        CS240 --> CS482
        CS343 --> CS374
        CS343 --> CS347
        CS343 --> CS447
       
        
        %%fourth
        CS361 --> CS450
        CS361 --> CS456
        CS361 --> CS470
        CS361 --> CS432
        CS361 --> CS455 %%check on that one
        CS361 --> CS457
        CS361 --> CS458
        CS457 --> CS458
        CS327 --> CS412
        CS327 --> CS452
        CS327 --> CS432
        CS327 --> CS445
        CS --> CS
        CS --> CS
        CS --> CS
        CS --> CS
        CS --> CS
        CS --> CS




        %%Special
        Permission  --> CS280
        Permission --> CS497
        Permission --> CS499
        CS240 --> CS444
       
    end
   
```