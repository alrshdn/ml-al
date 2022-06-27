# AI-Machine-Learning
## For using HDF5 formatted models:
>"Compared to the SavedModel format, there are two things that don't get included in the H5 file:

>* External losses & metrics added via model.add_loss() & model.add_metric() are not saved (unlike SavedModel). If you have such losses & metrics on your model and you want to resume training, you need to add these losses back yourself after loading the model. Note that this does not apply to losses/metrics created inside layers via self.add_loss() & self.add_metric(). As long as the layer gets loaded, these losses & metrics are kept, since they are part of the call method of the layer.
>* The computation graph of custom objects such as custom layers is not included in the saved file. At loading time, Keras will need access to the Python classes/functions of these objects in order to reconstruct the model. 
See Custom objects: https://www.tensorflow.org/guide/keras/save_and_serialize#custom-objects"

Source: https://www.tensorflow.org/guide/keras/save_and_serialize
