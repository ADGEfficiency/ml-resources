https://twitter.com/karpathy/status/1013244313327681536?lang=en

Most common neural net mistakes: 

1) you didn't try to overfit a single batch first. 
2) you forgot to toggle train/eval mode for the net. 
3) you forgot to .zero_grad() (in pytorch) before .backward(). 
4) you passed softmaxed outputs to a loss that expects raw logits. ; others? :)
