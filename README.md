# Batteries Remaining Useful Lifetime (RUL) prediction
(Data publicly available here: https://doi.org/10.1038/s41560-019-0356-8)

Here I report some models I've made in order to predict battery lifetimes based on a Recurrent Neural Network (RNN) architecture, based on timeseries-type data of battery charge/discharge cycles until failure. Lifetime is defined as the number of cycles until battery capacit degrades to 80% of its nominal starting value. 

The aim here is just to use windows of few cycles to predict the remaining battery lifetime, at any point during battery life. 

These models are results from a very simple, first-order grid-search-type investigation. Even considering that, the results look promising at this stage, with absolute errors on RUL on the order of 10-20 cycles. 

In order to obtain the very best model, a more thorough investigation is in order, and that's the scope of future work (mostly because higher computatinal resources are needed to train more complex models). It's also straightforward to modify the scripts to run on GPUs. 
