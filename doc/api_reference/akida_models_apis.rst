
Akida models API
================

.. automodule:: akida_models
    :members:

    Layer blocks
    ============

    CNN blocks
    ----------
    .. autofunction:: akida_models.layer_blocks.conv_block
    .. autofunction:: akida_models.layer_blocks.separable_conv_block
    .. autofunction:: akida_models.layer_blocks.dense_block

    Transformers blocks
    -------------------
    .. autofunction:: akida_models.layer_blocks.mlp_block
    .. autofunction:: akida_models.layer_blocks.multi_head_attention
    .. autofunction:: akida_models.layer_blocks.transformer_block

    Transposed blocks
    -----------------
    .. autofunction:: akida_models.layer_blocks.conv_transpose_block
    .. autofunction:: akida_models.layer_blocks.sepconv_transpose_block

    Detection block
    ---------------
    .. autofunction:: akida_models.layer_blocks.yolo_head_block

    Helpers
    =======

    Gamma constraint
    ----------------
    .. autofunction:: add_gamma_constraint

    Unfusing SeparableConvolutional
    -------------------------------
    .. autofunction:: unfuse_sepconv2d

    Extract samples
    ---------------
    .. autofunction:: extract_samples


    Knowledge distillation
    ======================

    .. autoclass:: akida_models.distiller.Distiller
    .. autoclass:: akida_models.distiller.DeitDistiller
    .. autofunction:: akida_models.distiller.KLDistillationLoss

    MACS
    ====
    .. autofunction:: akida_models.macs.get_flops
    .. autofunction:: akida_models.macs.display_macs

    Model I/O
    =========
    .. autofunction:: akida_models.model_io.load_model
    .. autofunction:: akida_models.model_io.load_weights
    .. autofunction:: akida_models.model_io.save_weights
    .. autofunction:: akida_models.model_io.get_model_path

    Utils
    =====
    .. autofunction:: akida_models.utils.fetch_file
    .. autofunction:: akida_models.utils.get_tensorboard_callback
    .. autofunction:: akida_models.utils.get_params_by_version

    Model zoo
    =========

    AkidaNet
    --------

    ImageNet
    ~~~~~~~~
    .. autofunction:: akida_models.akidanet_imagenet
    .. autofunction:: akida_models.akidanet_imagenet_pretrained
    .. autofunction:: akida_models.akidanet_edge_imagenet
    .. autofunction:: akida_models.akidanet_edge_imagenet_pretrained
    .. autofunction:: akida_models.akidanet18_imagenet
    .. autofunction:: akida_models.akidanet18_imagenet_pretrained
    .. autofunction:: akida_models.akidanet_faceidentification_pretrained
    .. autofunction:: akida_models.akidanet_faceidentification_edge_pretrained
    .. autofunction:: akida_models.akidanet_plantvillage_pretrained
    .. autofunction:: akida_models.akidanet_vww_pretrained

    Preprocessing
    *************
    .. autofunction:: akida_models.imagenet.preprocessing.preprocess_image
    .. autofunction:: akida_models.imagenet.preprocessing.index_to_label

    Mobilenet
    ---------

    ImageNet
    ~~~~~~~~
    .. autofunction:: akida_models.mobilenet_imagenet
    .. autofunction:: akida_models.mobilenet_imagenet_pretrained

    DS-CNN
    ------

    KWS
    ~~~
    .. autofunction:: akida_models.ds_cnn_kws
    .. autofunction:: akida_models.ds_cnn_kws_pretrained

    Preprocessing
    *************
    .. autofunction:: akida_models.kws.preprocessing.prepare_model_settings
    .. autofunction:: akida_models.kws.preprocessing.prepare_words_list
    .. autofunction:: akida_models.kws.preprocessing.which_set
    .. autoclass:: akida_models.kws.preprocessing.AudioProcessor
        :members:

    VGG
    ---

    UTK Face
    ~~~~~~~~
    .. autofunction:: akida_models.vgg_utk_face
    .. autofunction:: akida_models.vgg_utk_face_pretrained

    Preprocessing
    *************
    .. autofunction:: akida_models.utk_face.preprocessing.load_data

    YOLO
    ----

    .. autofunction:: akida_models.yolo_base
    .. autofunction:: akida_models.yolo_widerface_pretrained
    .. autofunction:: akida_models.yolo_voc_pretrained

    YOLO Toolkit
    ~~~~~~~~~~~~

    Processing
    **********
    .. autofunction:: akida_models.detection.processing.load_image
    .. autofunction:: akida_models.detection.processing.preprocess_image
    .. autofunction:: akida_models.detection.processing.decode_output
    .. autofunction:: akida_models.detection.processing.parse_voc_annotations
    .. autofunction:: akida_models.detection.processing.parse_widerface_annotations
    .. autoclass:: akida_models.detection.processing.BoundingBox
        :members:

    Performance
    ***********
    .. autoclass:: akida_models.detection.map_evaluation.MapEvaluation
        :members:

    Anchors
    *******
    .. autofunction:: akida_models.detection.generate_anchors.generate_anchors

    BatchGenerator
    **************
    .. autofunction:: akida_models.detection.batch_generator.BatchGenerator
    .. autofunction:: akida_models.detection.batch_generator.BatchYoloGenerator

    Utils
    *****
    .. autofunction:: akida_models.detection.box_utils.xywh_to_xyxy
    .. autofunction:: akida_models.detection.box_utils.xyxy_to_xywh
    .. autofunction:: akida_models.detection.box_utils.compute_overlap

    PointNet++
    ----------

    ModelNet40
    ~~~~~~~~~~
    .. autofunction:: akida_models.pointnet_plus_modelnet40
    .. autofunction:: akida_models.pointnet_plus_modelnet40_pretrained

    Processing
    **********
    .. autofunction:: akida_models.modelnet40.preprocessing.get_modelnet_from_file
    .. autofunction:: akida_models.modelnet40.preprocessing.get_modelnet

    GXNOR
    -----

    MNIST
    ~~~~~
    .. autofunction:: akida_models.gxnor_mnist
    .. autofunction:: akida_models.gxnor_mnist_pretrained

    CenterNet
    ---------
    .. autofunction:: akida_models.centernet_base
    .. autofunction:: akida_models.centernet_voc_pretrained
    .. autofunction:: akida_models.centernet.centernet_processing.decode_output
    .. autoclass:: akida_models.centernet.centernet_loss.CenternetLoss
    .. autoclass:: akida_models.centernet.centernet_batch_generator.BatchCenternetGenerator

    AkidaUNet
    ---------
    .. autofunction:: akida_models.akida_unet_portrait128
    .. autofunction:: akida_models.akida_unet_portrait128_pretrained

    Transformers
    ------------

    ViT
    ~~~
    .. autofunction:: akida_models.vit_imagenet
    .. autofunction:: akida_models.vit_ti16
    .. autofunction:: akida_models.bc_vit_ti16
    .. autofunction:: akida_models.bc_vit_ti16_imagenet_pretrained
    .. autofunction:: akida_models.vit_s16
    .. autofunction:: akida_models.vit_s32
    .. autofunction:: akida_models.vit_b16
    .. autofunction:: akida_models.vit_b32
    .. autofunction:: akida_models.vit_l16
    .. autofunction:: akida_models.vit_l32

    DeiT
    ~~~~
    .. autofunction:: akida_models.deit_imagenet
    .. autofunction:: akida_models.deit_ti16
    .. autofunction:: akida_models.bc_deit_ti16
    .. autofunction:: akida_models.bc_deit_dist_ti16_imagenet_pretrained
    .. autofunction:: akida_models.deit_s16
    .. autofunction:: akida_models.deit_b16
