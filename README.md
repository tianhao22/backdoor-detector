# backdoor-detector

## I.Project details
### Author: 
Tianhao Wang

### Goal: 
Design a backdoor detector for BadNets trained on the YouTube Face dataset using the pruning defense.
    
    ├── data 
        └── clean_validation_data.h5 // this is clean data used to evaluate the BadNet and design the backdoor defense
        └── clean_test_data.h5
        └── sunglasses_poisoned_data.h5
        └── anonymous_1_poisoned_data.h5
        └── multi-trigger_multi-target
            └── eyebrows_poisoned_data.h5
            └── lipstick_poisoned_data.h5
            └── sunglasses_poisoned_data.h5
    
    ├── GoodNets
        └── eval_anonymous_1.py //anonymous_1_bd_net.h5
        └── eval_anonymous_2.py //anonymous_2_bd_net.h5
        └── eval_multi.py //multi_trigger_multi_target_bd_net.h5
        └── eval_sunglasses.py // Goodnet for sunglasses_bd_net.h5
    
    ├── models
        └── sunglasses_bd_net.h5
        └── sunglasses_bd_weights.h5
        └── multi_trigger_multi_target_bd_net.h5
        └── multi_trigger_multi_target_bd_weights.h5
        └── anonymous_1_bd_net.h5
        └── anonymous_1_bd_weights.h5
        └── anonymous_2_bd_net.h5
        └── anonymous_2_bd_weights.h5
    
##II. Dependencies
1. Python 3.6.9
2. Keras 2.3.1
3. Numpy 1.16.3
4. Matplotlib 2.2.2
5. H5py 2.9.0
6. TensorFlow-gpu 1.15.2
     
