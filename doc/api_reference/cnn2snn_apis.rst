
CNN2SNN Toolkit API
===================

.. automodule:: cnn2snn

    Akida version
    =============
    .. autoclass:: AkidaVersion

        .. autodata:: cnn2snn.AkidaVersion.v1
            :annotation: =Akida 1.0 SOC and IP

        .. autodata:: cnn2snn.AkidaVersion.v2
            :annotation: =Akida 2.0 IP

    .. autofunction:: get_akida_version
    .. autofunction:: set_akida_version

    Conversion
    ==========
    .. autofunction:: convert

    A detailed description of the input_scaling parameter is given in the
    `user guide <../user_guide/cnn2snn.html#input-scaling>`__.

    .. autofunction:: cnn2snn.quantizeml.compatibility_checks.check_model_compatibility

    Legacy quantization API
    =======================

    While it is possible to quantize Akida 1.0 models using cnn2snn legacy quantization blocks, such
    usage is deprecated. You should rather use
    `QuantizeML <../user_guide/quantizeml.html#>`__ tool to quantize a model whenever possible.

    Utils
    -----
    .. autofunction:: check_model_compatibility
    .. autofunction:: load_quantized_model

    Calibration
    -----------
    .. autofunction:: cnn2snn.calibration.QuantizationSampler
    .. autofunction:: cnn2snn.calibration.bias_correction
    .. autofunction:: cnn2snn.calibration.adaround

    Transforms
    ----------
    .. autofunction:: cnn2snn.transforms.sequentialize
    .. autofunction:: cnn2snn.transforms.syncretize
    .. autofunction:: cnn2snn.transforms.invert_batchnorm_pooling
    .. autofunction:: cnn2snn.transforms.fold_batchnorm
    .. autofunction:: cnn2snn.transforms.weights_homogeneity
    .. autofunction:: cnn2snn.transforms.normalize_separable_layer
    .. autofunction:: cnn2snn.transforms.normalize_separable_model
    .. autofunction:: cnn2snn.transforms.reshape

    Constraint
    ----------
    .. autoclass:: cnn2snn.min_value_constraint.MinValueConstraint

    Quantization
    ------------
    .. autofunction:: quantize
    .. autofunction:: quantize_layer

    Quantizers
    ----------

    WeightQuantizer
    ~~~~~~~~~~~~~~~
    .. autoclass:: cnn2snn.quantization_ops.WeightQuantizer
        :members:
        :show-inheritance:

    LinearWeightQuantizer
    ~~~~~~~~~~~~~~~~~~~~~
    .. autoclass:: cnn2snn.quantization_ops.LinearWeightQuantizer
        :members:
        :show-inheritance:

    StdWeightQuantizer
    ~~~~~~~~~~~~~~~~~~
    .. autoclass:: StdWeightQuantizer
        :members:
        :show-inheritance:

    StdPerAxisQuantizer
    ~~~~~~~~~~~~~~~~~~~
    .. autoclass:: StdPerAxisQuantizer
        :members:
        :show-inheritance:

    MaxQuantizer
    ~~~~~~~~~~~~
    .. autoclass:: MaxQuantizer
        :members:
        :show-inheritance:

    MaxPerAxisQuantizer
    ~~~~~~~~~~~~~~~~~~~
    .. autoclass:: MaxPerAxisQuantizer
        :members:
        :show-inheritance:

    Quantized layers
    ----------------

    QuantizedConv2D
    ~~~~~~~~~~~~~~~
    .. autoclass:: QuantizedConv2D
        :members:
        :show-inheritance:

    QuantizedDense
    ~~~~~~~~~~~~~~
    .. autoclass:: QuantizedDense
        :members:
        :show-inheritance:

    QuantizedSeparableConv2D
    ~~~~~~~~~~~~~~~~~~~~~~~~
    .. autoclass:: QuantizedSeparableConv2D
        :members:
        :show-inheritance:

    QuantizedActivation
    ~~~~~~~~~~~~~~~~~~~
    .. autoclass:: QuantizedActivation
        :members:
        :show-inheritance:

    ActivationDiscreteRelu
    ~~~~~~~~~~~~~~~~~~~~~~
    .. autoclass:: ActivationDiscreteRelu
        :members:
        :show-inheritance:

    QuantizedReLU
    ~~~~~~~~~~~~~
    .. autoclass:: QuantizedReLU
        :members:
        :show-inheritance:
