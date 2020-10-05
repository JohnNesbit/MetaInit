# MetaInit
Uses meta neural network to create initialization weights for another network.
It works by feeding one input and one needed output to a first meta network.
Once this network has a loss of 0 then a network will be trained to cobble together 100
of these one sample size weights to fit all 100 inputs and outputs. This 100 sample wieght
is used as the initialization weight for a neural network. The reason the weight is limited to 100
is because it is just a rough approximation and anything more is too computationally expensive.
