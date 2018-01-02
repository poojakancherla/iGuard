# iGuard
This application automatically detects criminal activities in a security footage, which can be used to reduce the response time in order to prevent the risk.

# Setup
- Install Python 3.5.3
- Install Tensorflow
  ```
  python -m pip install tensorflow
  ```
- Clone the Tensorflow repository from codelabs
  ```
  git clone https://github.com/googlecodelabs/tensorflow-for-poets-2
  ```
# Training
```
python35 -m tensorflow-for-poets-2.scripts.retrain
    --bottleneck_dir=tf_files/bottlenecks
    --how_many_training_steps=5000
    --model_dir=tf_files/models/
    --summaries_dir=tf_files/training_summaries/"mobilenet_0.50_224"
    --output_graph=tf_files/retrained_graph.pb
    --output_labels=tf_files/retrained_labels.txt --architecture="mobilenet_0.50_224"
    --image_dir=tf_files/trainData

```

# 
