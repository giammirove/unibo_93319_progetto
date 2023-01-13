### MODELLO

```
__________________________________________________________________________________________________
 Layer (type)                   Output Shape         Param #     Connected to                     
==================================================================================================
 input_1 (InputLayer)           [(None, 1)]          0           []                               
                                                                                                  
 input_2 (InputLayer)           [(None, 1)]          0           []                               
                                                                                                  
 dense (Dense)                  (None, 2)            4           ['input_1[0][0]']                
                                                                                                  
 dense_1 (Dense)                (None, 2)            4           ['input_2[0][0]']                
                                                                                                  
 concatenate (Concatenate)      (None, 4)            0           ['dense[0][0]',                  
                                                                  'dense_1[0][0]']                
                                                                                                  
 dense_2 (Dense)                (None, 4)            20          ['concatenate[0][0]']            
                                                                                                  
 dense_3 (Dense)                (None, 4)            20          ['dense_2[0][0]']                
                                                                                                  
 dense_4 (Dense)                (None, 100)          500         ['dense_3[0][0]']                
                                                                                                  
==================================================================================================
Total params: 548
Trainable params: 548
Non-trainable params: 0
__________________________________________________________________________________________________

```
