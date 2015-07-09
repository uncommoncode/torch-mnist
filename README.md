# torch-mnist
A simple example of using common packages with torch to train a (low performing) neural network on the MNIST dataset.

I would suggest using this as a low-level template getting familiar with training feed-forward neural networks with torch. It doesn't provide any typical niceties of production code like encapsulation, modularity, or code reuse.

# Running

After torch is instaled, you can simply execute:

```
th train.lua
```

It will download MNIST data for torch and train a naive feed forward neural network with three layers:

1. Input Layer: `728 x 100` (takes in an flattened binary raster image)
2. Hidden Layer: `100 x 100`
3. Output Layer: `100 x 10` (outputs 10 possible classes; one for each digit 0-9. You can argmax this output to determine which class is determined to be most likely)

This is not a state of the art neural network. **Model performance is low, around 0.75 accuracy. There are many better models that you can implement; this is intentionally simple.**
