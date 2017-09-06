# RN1015k500
RN1015k500.mlmodel - Apple [Core ML](https://developer.apple.com/machine-learning/) model generated from the Apache MXNet model "[LocationNet](https://mxnet.incubator.apache.org/model_zoo/)".

## Instructions

On macOS, download the 4 files RN1015k500.aa, RN1015k500.ab, RN1015k500.ac and RN1015k500.ad to the same directory and run this command to create the file RN1015k500.mlmodel:

```sh
$ cat RN1015k500.aa RN1015k500.ab RN1015k500.ac RN1015k500.ad > RN1015k500.mlmodel
```

Then to verify the integrity of the file RN1015k500.mlmodel, run the following command and visually confirm that the resulting hash is 6d59a68b9be7a14705aba0bd957f72b0fef29cd2

```sh
$ openssl sha1 RN1015k500.mlmodel
```


## Note
RN1015k500.mlmodel was generated using the [MXNet to Core ML converter tool](https://github.com/apache/incubator-mxnet/tree/master/tools/coreml) with the following command:

```sh
$ mxnet_coreml_converter.py --model-prefix='RN101-5k500' --epoch=12 --input-shape='{"data":"3,224,224"}' --mode=classifier --pre-processing-arguments='{"image_input_names":"data"}' --class-labels grids.txt --output-file="RN1015k500.mlmodel"
```
