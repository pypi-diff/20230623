# Comparing `tmp/seqexplainer-0.0.1.tar.gz` & `tmp/seqexplainer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqexplainer-0.0.1.tar", max compression
+gzip compressed data, was "seqexplainer-0.1.0.tar", max compression
```

## Comparing `seqexplainer-0.0.1.tar` & `seqexplainer-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,28 @@
--rw-r--r--   0        0        0     1066 2022-12-20 00:45:44.000000 seqexplainer-0.0.1/LICENSE
--rw-r--r--   0        0        0      443 2023-01-26 05:09:16.000000 seqexplainer-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      223 2023-01-26 05:09:25.000000 seqexplainer-0.0.1/seqexplainer/__init__.py
--rw-r--r--   0        0        0     2239 2023-01-26 04:56:41.000000 seqexplainer-0.0.1/seqexplainer/_dim_reduction.py
--rw-r--r--   0        0        0    10020 2023-01-26 04:56:08.000000 seqexplainer-0.0.1/seqexplainer/_feature_attribution.py
--rw-r--r--   0        0        0    13869 2022-12-20 00:50:12.000000 seqexplainer-0.0.1/seqexplainer/_filter_viz.py
--rw-r--r--   0        0        0    12413 2022-12-20 00:45:44.000000 seqexplainer-0.0.1/seqexplainer/_in_silico.py
--rw-r--r--   0        0        0     4168 2022-12-20 00:45:44.000000 seqexplainer-0.0.1/seqexplainer/_moana.py
--rw-r--r--   0        0        0     2149 2023-01-26 04:54:50.000000 seqexplainer-0.0.1/seqexplainer/_references.py
--rw-r--r--   0        0        0    22833 2023-01-26 04:54:12.000000 seqexplainer-0.0.1/seqexplainer/_seq.py
--rw-r--r--   0        0        0     6018 2022-12-29 23:59:59.000000 seqexplainer-0.0.1/seqexplainer/_utils.py
--rw-r--r--   0        0        0      750 2023-01-26 05:16:18.909304 seqexplainer-0.0.1/setup.py
--rw-r--r--   0        0        0      600 2023-01-26 05:16:18.909635 seqexplainer-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-03-26 17:51:58.000000 seqexplainer-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1992 2023-03-26 17:52:14.000000 seqexplainer-0.1.0/README.md
+-rw-r--r--   0        0        0      455 2023-06-23 19:43:20.000000 seqexplainer-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      211 2023-06-06 17:16:19.000000 seqexplainer-0.1.0/seqexplainer/__init__.py
+-rw-r--r--   0        0        0     2529 2023-06-06 16:07:43.000000 seqexplainer-0.1.0/seqexplainer/_ism.py
+-rw-r--r--   0        0        0     2815 2023-06-05 00:05:42.000000 seqexplainer-0.1.0/seqexplainer/_layer_outs.py
+-rw-r--r--   0        0        0     3959 2023-06-03 00:23:20.000000 seqexplainer-0.1.0/seqexplainer/_plot.py
+-rw-r--r--   0        0        0     4628 2023-06-04 23:37:23.000000 seqexplainer-0.1.0/seqexplainer/_utils.py
+-rw-r--r--   0        0        0       75 2023-06-03 00:40:39.000000 seqexplainer-0.1.0/seqexplainer/attributions/__init__.py
+-rw-r--r--   0        0        0     3443 2023-06-06 17:00:58.000000 seqexplainer-0.1.0/seqexplainer/attributions/_attributions.py
+-rw-r--r--   0        0        0     7568 2023-06-03 00:23:20.000000 seqexplainer-0.1.0/seqexplainer/attributions/_modisco.py
+-rw-r--r--   0        0        0    10017 2023-06-03 00:45:03.000000 seqexplainer-0.1.0/seqexplainer/attributions/_references.py
+-rw-r--r--   0        0        0     4242 2023-06-03 00:23:20.000000 seqexplainer-0.1.0/seqexplainer/deprecated/_deprecated.py
+-rw-r--r--   0        0        0    11640 2023-03-26 19:16:55.000000 seqexplainer-0.1.0/seqexplainer/experimental/_experimental.py
+-rw-r--r--   0        0        0       84 2023-06-07 00:01:45.000000 seqexplainer-0.1.0/seqexplainer/filters/__init__.py
+-rw-r--r--   0        0        0     3246 2023-06-08 22:08:16.000000 seqexplainer-0.1.0/seqexplainer/filters/_filters.py
+-rw-r--r--   0        0        0     1892 2023-06-03 00:40:56.000000 seqexplainer-0.1.0/seqexplainer/filters/_motifs.py
+-rw-r--r--   0        0        0       33 2023-06-06 05:20:04.000000 seqexplainer-0.1.0/seqexplainer/generative/__init__.py
+-rw-r--r--   0        0        0     6155 2023-06-06 17:00:53.000000 seqexplainer-0.1.0/seqexplainer/generative/_evolution.py
+-rw-r--r--   0        0        0       39 2023-06-06 17:09:25.000000 seqexplainer-0.1.0/seqexplainer/gia/__init__.py
+-rw-r--r--   0        0        0     5178 2023-06-22 20:45:23.000000 seqexplainer-0.1.0/seqexplainer/gia/_complex_perturb.py
+-rw-r--r--   0        0        0     3971 2023-06-22 17:36:55.000000 seqexplainer-0.1.0/seqexplainer/gia/_gia.py
+-rw-r--r--   0        0        0        0 2023-06-22 17:08:33.000000 seqexplainer-0.1.0/seqexplainer/gia/_gia_helpers.py
+-rw-r--r--   0        0        0     2459 2023-06-03 00:41:26.000000 seqexplainer-0.1.0/seqexplainer/gia/_null_models.py
+-rw-r--r--   0        0        0    16623 2023-06-22 17:08:05.000000 seqexplainer-0.1.0/seqexplainer/gia/_perturb.py
+-rw-r--r--   0        0        0     9445 2023-06-03 00:38:33.000000 seqexplainer-0.1.0/seqexplainer/preprocess/_helpers.py
+-rw-r--r--   0        0        0    13895 2023-06-03 00:38:34.000000 seqexplainer-0.1.0/seqexplainer/preprocess/_preprocess.py
+-rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 seqexplainer-0.1.0/PKG-INFO
```

### Comparing `seqexplainer-0.0.1/LICENSE` & `seqexplainer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seqexplainer-0.0.1/seqexplainer/_feature_attribution.py` & `seqexplainer-0.1.0/seqexplainer/experimental/_experimental.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,286 +1,352 @@
 import torch
+from torch.optim import Adam
+
+import os
+import logging
+import torch
+import torch.nn as nn
 import numpy as np
-from typing import Union, Callable
-from tqdm.auto import tqdm
-from captum.attr import InputXGradient, DeepLift, GradientShap, DeepLiftShap
-from ._references import _get_reference
-from ._utils import _model_to_device, _naive_ism
-from eugene import settings as settings
-
-# In silico mutagenesis methods
-ISM_REGISTRY = {
-    "NaiveISM": _naive_ism,
-}
-
-def _ism_attributions(
-    model: torch.nn.Module, 
-    inputs: tuple, 
-    method: Union[str, Callable],
-    target: int = 0,
-    device: str = "cpu", 
-    **kwargs
-):
-    if isinstance(inputs, torch.Tensor):
-        inputs = inputs.detach().cpu().numpy()
-    if model.strand != "ss":
-        raise ValueError("ISM currrently only works for single strand models, but we are working on this!")
-    attrs = ISM_REGISTRY[method](
-        model=model,
-        X_0=inputs,  # Rename to inputs eventually
-        device=device,
-        **kwargs
-    )
-    return attrs
-
-# Captum methods
-CAPTUM_REGISTRY = {
-    "InputXGradient": InputXGradient,
-    "DeepLift": DeepLift,
-    "DeepLiftShap": DeepLiftShap,
-    "GradientShap": GradientShap,
-
-}
-
-def _captum_attributions(
-    model: torch.nn.Module,
-    inputs: tuple,
-    method: str,
-    target: int = 0,
-    **kwargs
-):
-    """
-    """
-    if isinstance(inputs, np.ndarray):
-        inputs = torch.tensor(inputs)
-    attributor = CAPTUM_REGISTRY[method](model)
-    attrs = attributor.attribute(inputs=inputs, target=target, **kwargs)
-    return attrs
-
-ATTRIBUTIONS_REGISTRY = {
-    "NaiveISM": _ism_attributions,
-    "InputXGradient": _captum_attributions,
-    "DeepLift": _captum_attributions,
-    "GradientShap": _captum_attributions,
-    "DeepLiftShap": _captum_attributions,
-}
-
-def attribute(
-    model,
-    inputs: torch.Tensor,
-    method: Union[str, Callable],
-    target: int = 0,
-    device: str = "cpu",
-    **kwargs
-):
-
-    # Set device
-    device = "cuda" if settings.gpus > 0 else "cpu" if device is None else device
-
-    # Put model on device
-    model = _model_to_device(model, device)
-
-    # Put inputs on device
-    if isinstance(inputs, tuple):
-        inputs = tuple([i.requires_grad_().to(device) for i in inputs])
+from yuzu.utils import perturbations
+
+
+# my own
+def generate_maximally_activating_input(model, neuron_index, input_size, lr=0.1, steps=100):
+    # Create a random input tensor with the specified size
+    input_tensor = torch.randn(input_size)
+    input_tensor.requiresGrad = True
+    
+    # Define the optimizer
+    optimizer = Adam([input_tensor], lr=lr)
+    
+    # Perform gradient ascent
+    for _ in range(steps):
+        optimizer.zero_grad()
+        output = model(input_tensor)
+        # get the output of the intermediate layer
+        intermediate_output = model.intermediate_layer(input_tensor)
+        # select the output of the neuron of interest
+        neuron_output = intermediate_output[0, neuron_index]
+        neuron_output.backward()
+        optimizer.step()
+    
+    return input_tensor
+
+#https://github.com/MedChaabane/deepRAM/blob/master/extract_motifs.py
+def plot_target_corr(filter_outs, seq_targets, filter_names, target_names, out_pdf, seq_op='mean'):
+    num_seqs = filter_outs.shape[0]
+    num_targets = len(target_names)
+
+    if seq_op == 'mean':
+        filter_outs_seq = filter_outs.mean(axis=2)
     else:
-        inputs = inputs.requires_grad_().to(device)
+        filter_outs_seq = filter_outs.max(axis=2)
 
-    # Check kwargs for reference
-    if "reference_type" in kwargs:
-        ref_type = kwargs.pop("reference_type")
-        kwargs["baselines"] = _get_reference(inputs, ref_type, device)
-
-    #print(inputs[0].requires_grad)#, kwargs["baselines"][0].requires_grad)
-    #print(inputs.shape, kwargs["baselines"].shape, kwargs["additional_forward_args"].shape)
-    #print(kwargs.keys(), method, target, model)
-    # Get attributions
-    attr = ATTRIBUTIONS_REGISTRY[method](
-        model=model,
-        inputs=inputs,
-        method=method,
-        target=target,
-        **kwargs
-    )
-
-    # Return attributions
-    return attr
-
-
-def feature_attribution_sdata(
-    model: torch.nn.Module,  # need to enforce this is a SequenceModel
-    sdata,
-    method: str = "DeepLiftShap",
-    target: int = 0,
-    aggr: str = None,
-    multiply_by_inputs: bool = True,
-    batch_size: int = None,
-    num_workers: int = None,
-    device: str = "cpu",
-    transform_kwargs: dict = {},
-    prefix: str = "",
-    suffix: str = "",
-    copy: bool = False,
-    **kwargs
-):
-    """
-    Wrapper function to compute feature attribution scores for a SequenceModel using the 
-    set of sequences defined in a SeqData object.
+    # std is sequence by filter.
+    filter_seqs_std = filter_outs_seq.std(axis=0)
+    filter_outs_seq = filter_outs_seq[:,filter_seqs_std > 0]
+    filter_names_live = filter_names[filter_seqs_std > 0]
+
+    filter_target_cors = np.zeros((len(filter_names_live),num_targets))
+    for fi in range(len(filter_names_live)):
+        for ti in range(num_targets):
+            cor, p = spearmanr(filter_outs_seq[:,fi], seq_targets[:num_seqs,ti])
+            filter_target_cors[fi,ti] = cor
+
+    cor_df = pd.DataFrame(filter_target_cors, index=filter_names_live, columns=target_names)
+
+    sns.set(font_scale=0.3)
+    plt.figure()
+    sns.clustermap(cor_df, cmap='BrBG', center=0, figsize=(8,10))
+    plt.savefig(out_pdf)
+    plt.close()
+
+#https://github.com/p-koo/tfomics/blob/master/tfomics/impress.py
+def plot_filters(W, fig, num_cols=8, alphabet='ACGT', names=None, fontsize=12):
+  """plot 1st layer convolutional filters"""
+
+  num_filter, filter_len, A = W.shape
+  num_rows = np.ceil(num_filter/num_cols).astype(int)
+
+  fig.subplots_adjust(hspace=0.2, wspace=0.2)
+  for n, w in enumerate(W):
+    ax = fig.add_subplot(num_rows,num_cols,n+1)
     
-    Allows for computing scores using different methods and different reference types on any task.
+    # Calculate sequence logo heights -- information
+    I = np.log2(4) + np.sum(w * np.log2(w+1e-7), axis=1, keepdims=True)
+    logo = I*w
+
+    # Create DataFrame for logomaker
+    counts_df = pd.DataFrame(data=0.0, columns=list(alphabet), index=list(range(filter_len)))
+    for a in range(A):
+      for l in range(filter_len):
+        counts_df.iloc[l,a] = logo[l,a]
+
+    logomaker.Logo(counts_df, ax=ax)
+    ax = plt.gca()
+    ax.set_ylim(0,2)
+    ax.spines['right'].set_visible(False)
+    ax.spines['top'].set_visible(False)
+    ax.yaxis.set_ticks_position('none')
+    ax.xaxis.set_ticks_position('none')
+    plt.xticks([])
+    plt.yticks([])
+    if names is not None:
+      plt.ylabel(names[n], fontsize=fontsize)
+
+# MOANA (MOtif ANAlysis)
+def activation_pwm(fmap, X, threshold=0.5, window=20):
+    # Set the left and right window sizes
+    window_left = int(window/2)
+    window_right = window - window_left
+
+    N, L, A = X.shape # assume this ordering (i.e., TensorFlow ordering) of channels in X
+    num_filters = fmap.shape[-1]
+
+    W = []
+    for filter_index in range(num_filters):
+
+        # Find regions above threshold
+        coords = np.where(fmap[:,:,filter_index] > np.max(fmap[:,:,filter_index])*threshold)
+        x, y = coords
+
+        # Sort score
+        index = np.argsort(fmap[x,y,filter_index])[::-1]
+        data_index = x[index].astype(int)
+        pos_index = y[index].astype(int)
+
+        # Make a sequence alignment centered about each activation (above threshold)
+        seq_align = []
+        for i in range(len(pos_index)):
+
+            # Determine position of window about each filter activation
+            start_window = pos_index[i] - window_left
+            end_window = pos_index[i] + window_right
+
+            # Check to make sure positions are valid
+            if (start_window > 0) & (end_window < L):
+                seq = X[data_index[i], start_window:end_window, :]
+                seq_align.append(seq)
+
+        # Calculate position probability matrix
+        if len(seq_align) > 0:
+            W.append(np.mean(seq_align, axis=0))
+        else:
+            W.append(np.zeros((window, A)))
+    W = np.array(W)
+
+    return W
+
+# MOANA (MOtif ANAlysis)
+def clip_filters(W, threshold=0.5, pad=3):
+    W_clipped = []
+    for w in W:
+        L, A = w.shape
+        entropy = np.log2(4) + np.sum(w*np.log2(w+1e-7), axis=1)
+        index = np.where(entropy > threshold)[0]
+        if index.any():
+            start = np.maximum(np.min(index)-pad, 0)
+            end = np.minimum(np.max(index)+pad+1, L)
+            W_clipped.append(w[start:end,:])
+        else:
+            W_clipped.append(w)
+
+    return W_clipped
+
+# MOANA (MOtif ANAlysis)
+def generate_meme(W, output_file='meme.txt', prefix='Filter'):
+    # background frequency
+    nt_freqs = [1./4 for i in range(4)]
+
+    # open file for writing
+    f = open(output_file, 'w')
+
+    # print intro material
+    f.write('MEME version 4\n')
+    f.write('\n')
+    f.write('ALPHABET= ACGT\n')
+    f.write('\n')
+    f.write('Background letter frequencies:\n')
+    f.write('A %.4f C  %.4f G %.4f T %.4f \n' % tuple(nt_freqs))
+    f.write('\n')
+
+    for j, pwm in enumerate(W):
+        if np.count_nonzero(pwm) > 0:
+            L, A = pwm.shape
+            f.write('MOTIF %s%d \n' % (prefix, j))
+            f.write('letter-probability matrix: alength= 4 w= %d nsites= %d \n' % (L, L))
+            for i in range(L):
+                f.write('%.4f %.4f %.4f %.4f \n' % tuple(pwm[i,:]))
+            f.write('\n')
+    
+    f.close()
+
+# MOANA (MOtif ANAlysis)
+def plot_filters(W, fig, num_cols=8, alphabet="ACGT", names=None, fontsize=12):
+    """plot first-layer convolutional filters from PWM"""
+    
+    if alphabet == "ATCG":
+        W = W[:,:,[0,2,3,1]]
     
+    num_filter, filter_len, A = W.shape
+    num_rows = np.ceil(num_filter/num_cols).astype(int)
+
+    fig.subplots_adjust(hspace=0.2, wspace=0.2)
+    for n, w in enumerate(W):
+        ax = fig.add_subplot(num_rows,num_cols,n+1)
+
+        # Calculate sequence logo heights -- information
+        I = np.log2(4) + np.sum(w * np.log2(w+1e-7), axis=1, keepdims=True)
+        logo = I*w
+        
+        # Create DataFrame for logomaker
+        counts_df = pd.DataFrame(data=0.0, columns=list(alphabet), index=list(range(filter_len)))
+        for a in range(A):
+            for l in range(filter_len):
+                counts_df.iloc[l,a] = logo[l,a]
+        
+        logomaker.Logo(counts_df, ax=ax)
+        ax = plt.gca()
+        ax.set_ylim(0, 2) # set y-axis of all sequence logos to run from 0 to 2 bits
+        ax.spines['right'].set_visible(False)
+        ax.spines['top'].set_visible(False)
+        ax.yaxis.set_ticks_position('none')
+        ax.xaxis.set_ticks_position('none')
+        plt.xticks([])
+        plt.yticks([])
+
+        if names:
+            plt.ylabel(names[n], fontsize=fontsize)
+        
+    return fig
+
+# peter koo
+def convert_tfr_to_np(tfr_dataset):
+    """
+    convert tfr dataset to a list of numpy arrays
+    :param tfr_dataset: tfr dataset format
+    :return:
+    """
+    all_data = [[] for i in range(len(next(iter(tfr_dataset))))]
+    for i, (data) in enumerate(tfr_dataset):
+        for j, data_type in enumerate(data):
+            all_data[j].append(data_type)
+    return [np.concatenate(d) for d in all_data]
+
+# peter koo
+def batch_np(whole_dataset, batch_size):
+    """
+    batch a np array for passing to a model without running out of memory
+    :param whole_dataset: np array dataset
+    :param batch_size: batch size
+    :return: generator of np batches
+    """
+    for i in range(0, whole_dataset.shape[0], batch_size):
+        yield whole_dataset[i:i + batch_size]
+
+# generative stuff
+def seqs_from_tensor(tensor : torch.tensor, num_seqs : int = 1) -> np.ndarray:
+    """
+    Decodes sequences represented by tensors into their string values.
+
     Parameters
     ----------
-    model : torch.nn.Module
-       PyTorch model to use for computing feature attribution scores.
-        Can be a EUGENe trained model or one you trained with PyTorch or PL.
-    sdata : SeqData
-        SeqData object containing the sequences to compute feature attribution scores on.
-    method: str
-        Type of saliency to use for computing feature attribution scores.
-        Can be one of the following:
-        - "gradxinput" (gradients x inputs)
-        - "intgrad" (integrated gradients)
-        - "intgradxinput" (integrated gradients x inputs)
-        - "smoothgrad" (smooth gradients)
-        - "smoothgradxinput" (smooth gradients x inputs)
-        - "deeplift" (DeepLIFT)
-        - "gradientshap" (GradientSHAP)
-    target: int
-        Index of the target class to compute scores for if there are multiple outputs. If there
-        is a single output, this should be None
-    batch_size: int
-        Batch size to use for computing feature attribution scores. If not specified, will use the
-        default batch size of the model
-    num_workers: int
-        Number of workers to use for computing feature attribution scores. If not specified, will use
-        the default number of workers of the model
-    device: str
-        Device to use for computing feature attribution scores.
-        EUGENe will always use a gpu if available
-    transform_kwargs: dict
-        Dictionary of keyword arguments to pass to the transform method of the model
-    prefix: str
-        Prefix to add to the feature attribution scores
-    suffix: str
-        Suffix to add to the feature attribution scores
-    copy: bool
-        Whether to copy the SeqData object before computing feature attribution scores. By default
-        this is False
-    **kwargs
-        Additional arguments to pass to the saliency method. For example, you can pass the number of
-        samples to use for SmoothGrad and Integrated Gradients
+    tensor : torch.tensor
+        Tensor to be decoded.
+    num_seqs : int
+        Number of sequences to decode.
+        Default is 1.
+
     Returns
     -------
-    SeqData
-        SeqData object containing the feature attribution scores
+    seqs : np.ndarray
+        Numpy array of decoded sequences.
     """
+    tokens = np.argmax(tensor.detach().numpy(), axis=1).reshape(num_seqs, -1)
+    seqs = np.array([decode_seq(_token2one_hot(token)) for token in tokens])
+    return seqs
 
-    # Disable cudnn for faster computations
-    torch.backends.cudnn.enabled = False
-    
-    # Copy the SeqData object if necessary
-    sdata = sdata.copy() if copy else sdata
+# EUGENe for generative models
+def latent_interpolation(latent_dim : int, samples : int, num_seqs : int = 1, generator = None, normal : bool = False, inclusive : bool = True) -> list:
+    """
+    Linearly interpolates between two random latent points. Useful for visualizing generative generators.
 
-    # Configure the device, batch size, and number of workers
-    device = "cuda" if settings.gpus > 0 else "cpu" if device is None else device
-    batch_size = batch_size if batch_size is not None else settings.batch_size
-    num_workers = num_workers if num_workers is not None else settings.dl_num_workers
-
-    # Make a dataloader from the sdata
-    sdataset = sdata.to_dataset(target_keys=None, transform_kwargs=transform_kwargs)
-    sdataloader = sdataset.to_dataloader(batch_size=batch_size, shuffle=False)
-    
-    # Create an empty array to hold attributions
-    dataset_len = len(sdataloader.dataset)
-    example_shape = sdataloader.dataset[0][1].numpy().shape
-    all_forward_explanations = np.zeros((dataset_len, *example_shape))
-    if model.strand != "ss":
-        all_reverse_explanations = np.zeros((dataset_len, *example_shape))
-
-    # Loop through batches and compute attributions
-    for i_batch, batch in tqdm(
-        enumerate(sdataloader),
-        total=int(dataset_len / batch_size),
-        desc=f"Computing saliency on batches of size {batch_size}",
-    ):
-        _, x, x_rev_comp, y = batch
-        if model.strand == "ss":
-            curr_explanations = attribute(
-                model,
-                x,
-                target=target,
-                method=method,
-                device=device,
-                additional_forward_args=x_rev_comp[0],
-                **kwargs,
-            )
-        else:
-            curr_explanations = attribute(
-                model,
-                (x, x_rev_comp),
-                target=target,
-                method=method,
-                device=device,
-                **kwargs,
-            )
-        if (i_batch+1)*batch_size < dataset_len:
-            if model.strand == "ss":
-                all_forward_explanations[i_batch*batch_size:(i_batch+1)*batch_size] = curr_explanations.detach().cpu().numpy()
-            else:
-                all_forward_explanations[i_batch*batch_size:(i_batch+1)*batch_size] = curr_explanations[0].detach().cpu().numpy()
-                all_reverse_explanations[i_batch * batch_size:(i_batch+1)*batch_size] = curr_explanations[1].detach().cpu().numpy()
-        else:
-            if model.strand == "ss":
-                all_forward_explanations[i_batch * batch_size:dataset_len] = curr_explanations.detach().cpu().numpy()
-            else:
-                all_forward_explanations[i_batch*batch_size:dataset_len] = curr_explanations[0].detach().cpu().numpy()
-                all_reverse_explanations[i_batch*batch_size:dataset_len] = curr_explanations[1].detach().cpu().numpy()
-    
-    # Add the attributions to sdata 
-    if model.strand == "ss":
-        sdata.uns[f"{prefix}{method}_imps{suffix}"] = all_forward_explanations
+    Parameters
+    ----------
+    latent_dim : int
+        Latent dimension of random latent space points.
+    samples : int
+        Number of samples to make between the two latent points. Higher numbers represent more sequences and should show smoother results.
+    num_seqs : int
+        Number of sequence channels to interpolate.
+        Defaults to 1.
+    generator : Basgeneratore
+        If provided, interpolated values will be passed through the given generator and be returned in place of latent points.
+        Default is None.
+    normal : bool
+        Whether to randomly sample points from a standard normal distibution rather than from 0 to 1.
+        Defaults to False.
+    inclusive : bool
+        Whether to returm random latent points along with their interpolated samples.
+        Defaults to True.
+
+    Returns
+    -------
+    z_list : list
+        List of latent space points represented as tensors.
+    gen_seqs : list
+        List of tokenized sequences expressed as strings.
+        Returns in place of z_list when a generator is provided.
+    """
+    if normal:
+        z1 = torch.normal(0, 1, (num_seqs, latent_dim))
+        z2 = torch.normal(0, 1, (num_seqs, latent_dim))
     else:
-        if aggr == "max":
-            sdata.uns[f"{prefix}{method}_imps{suffix}"] = np.maximum(all_forward_explanations, all_reverse_explanations)
-        elif aggr == "mean":
-            sdata.uns[f"{prefix}{method}_imps{suffix}"] = (all_forward_explanations + all_reverse_explanations) / 2
-        elif aggr == None:
-            sdata.uns[f"{prefix}{method}_forward_imps{suffix}"] = all_forward_explanations
-            sdata.uns[f"{prefix}{method}_reverse_imps{suffix}"] = all_reverse_explanations
-    return sdata if copy else None
-
-def aggregate_importances_sdata(
-    sdata, 
-    uns_key,
-    copy=False
-):
+        z1 = torch.rand(num_seqs, latent_dim)
+        z2 = torch.rand(num_seqs, latent_dim)
+
+    z_list = []
+    for n in range(samples):
+        weight = (n + 1)/(samples + 1)
+        z_interp = torch.lerp(z1, z2, weight)
+        z_list.append(z_interp)
+    if inclusive:
+        z_list.insert(0, z1)
+        z_list.append(z2)
+
+    if generator is None:
+        return z_list
+
+    gen_seqs = []
+    for z in z_list:
+        gen_seq = seqs_from_tensor(generator(z))
+        gen_seqs.append(gen_seq)
+    return gen_seqs
+
+# EUGENe for generative models
+def generate_seqs_from_generator(generator, num_seqs : int = 1, normal : bool = False, device : str = "cpu"):
     """
-    Aggregate feature attribution scores for a SeqData
-    
-    This function aggregates the feature attribution scores for a SeqData object
+    Generates random sequences from a generative generator.
+
     Parameters
     ----------
-    sdata : SeqData
-        SeqData object
-    uns_key : str
-        Key in the uns attribute of the SeqData object to use as feature attribution scores
-    """
-    sdata = sdata.copy() if copy else sdata
-    vals = sdata.uns[uns_key]
-    df = sdata.pos_annot.df
-    agg_scores = []
-    for i, row in df.iterrows():
-        seq_id = row["Chromosome"]
-        start = row["Start"]
-        end = row["End"]
-        seq_idx = np.where(sdata.names == seq_id)[0][0]
-        agg_scores.append(vals[seq_idx, :, start:end].sum())
-    df[f"{uns_key}_agg_scores"] = agg_scores
-    ranges = pr.PyRanges(df)
-    sdata.pos_annot = ranges
-    return sdata if copy else None
+    generator : Basgeneratore
+        Generative generator used for sequence generation.
+    num_seqs : int
+        Number of sequences to decode.
+        Default is 1.
+    normal : bool
+        Whether to sample from a normal distribution instead of a uniform distribution.
+        Default is false.
 
-def tfmodisco_sdata(
-    
-):
-    print("Cmon")
+    Returns
+    -------
+    seqs : np.ndarray
+        Numpy array of decoded sequences.
+    """
+    if normal:
+        z = torch.Tensor(np.random.normal(0, 1, (num_seqs, generator.latent_dim)))
+    else: 
+        z = torch.rand(num_seqs, generator.latent_dim)
+    z = z.to(device)
+    fake = generator(z)
+    return seqs_from_tensor(fake.cpu(), num_seqs)
```

### Comparing `seqexplainer-0.0.1/seqexplainer/_in_silico.py` & `seqexplainer-0.1.0/seqexplainer/preprocess/_preprocess.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,351 +1,453 @@
-import torch
-import numpy as np
 from tqdm.auto import tqdm
-from ._utils import _k_largest_index_argsort, _naive_ism
-from ..preprocess import ohe_seqs, feature_implant_across_seq
-from ..utils import track
-from .. import settings
-
-
-def best_k_muts(
-    model: torch.nn.Module, 
-    X: np.ndarray, 
-    k: int = 1, 
-    device: str = None
-) -> np.ndarray:
-    """
-    Find and return the k highest scoring sequence from referenece sequence X.
-
-    Using ISM, this function calculates all the scores of all possible mutations
-    of the reference sequence using a trained model. It then returns the k highest
-    scoring sequences, along with delta scores from the reference sequence and the indeces
-    along the lengths of the sequences where the mutations can be found
+import pandas as pd
+import numpy as np
+import torch
+from ._helpers import (
+    _tokenize,
+    _sequencize,
+    _token2one_hot,
+    _one_hot2token,
+    _pad_sequences,
+)  # modified concise
+from ._helpers import (
+    _string_to_char_array,
+    _one_hot_to_tokens,
+    _char_array_to_string,
+    _tokens_to_one_hot,
+)  # dinuc_shuffle
+
+
+# Vocabularies
+DNA = ["A", "C", "G", "T"]
+RNA = ["A", "C", "G", "U"]
+COMPLEMENT_DNA = {"A": "T", "C": "G", "G": "C", "T": "A"}
+COMPLEMENT_RNA = {"A": "U", "C": "G", "G": "C", "U": "A"}
+
+
+def sanitize_seq(seq):
+    """Capitalizes and removes whitespace for single seq."""
+    return seq.strip().upper()
+
+
+def sanitize_seqs(seqs):
+    """Capitalizes and removes whitespace for a set of sequences."""
+    return np.array([seq.strip().upper() for seq in seqs])
 
-    Parameters
-    ----------
-    model: torch.nn.Module
-        The model to score the sequences with
-    X: np.ndarray
-        The one-hot encoded sequence to calculate find mutations for.
-    k: int, optional
-        The number of mutated seqences to return
-    device: str, optional
-        Whether to use a 'cpu' or 'cuda'.
 
-    Returns
-    -------
-    mut_X: np.ndarray
-        The k highest scoring one-hot-encoded sequences
-    maxs: np.ndarray
-        The k highest delta scores corresponding to the k highest scoring sequences
-    locs: np.ndarray
-        The indeces along the length of the sequences where the mutations can be found
-    """
-    device = "cuda" if settings.gpus > 0 else "cpu" if device is None else device
-    model.eval().to(device)
-    X = np.expand_dims(X, axis=0) if X.ndim == 2 else X
-    X = X.transpose(0, 2, 1) if X.shape[2] == 4 else X
-    X = torch.Tensor(X).float().numpy()
-    X_ism = _naive_ism(model, X, device=device, batch_size=1)
-    X_ism = X_ism.squeeze(axis=0)
-    inds = _k_largest_index_argsort(X_ism, k)
-    locs = inds[:, 1]
-    maxs = np.max(X_ism, axis=0)[locs]
-    mut_Xs = np.zeros((k, X.shape[1], X.shape[2]))
-    for i in range(k):
-        mut_X = X.copy().squeeze(axis=0)
-        mut_X[:, inds[i][1]] = np.zeros(mut_X.shape[0])
-        mut_X[:, inds[i][1]][inds[i][0]] = 1
-        mut_Xs[i] = mut_X
-    return mut_Xs, maxs, locs
-
-
-def best_mut_seqs(
-    model: torch.nn.Module,
-    X: np.ndarray, 
-    batch_size: int = None, 
-    device: str = None
-) -> np.ndarray:
-    """Find and return the highest scoring sequence for each sequence from a set reference sequences X. 
-    
-    X should contain one-hot-encoded sequences
-    and should be of shape (n, 4, l). n is the number of sequences, 4 is the number of
-    nucleotides, and l is the length of the sequence.
-
-    Using ISM, this function calculates all the scores of all possible mutations
-    of each reference sequence using a trained model. It then returns the highest
-    scoring sequence, along with delta scores from the reference sequence and the indeces
-    along the lengths of the sequences where the mutations can be found.
+def ascii_encode_seq(seq, pad=0):
+    """
+    Converts a string of characters to a NumPy array of byte-long ASCII codes.
+    """
+    encode_seq = np.array([ord(letter) for letter in seq], dtype=int)
+    if pad > 0:
+        encode_seq = np.pad(
+            encode_seq, pad_width=(0, pad), mode="constant", constant_values=36
+        )
+    return encode_seq
+
+
+def ascii_encode_seqs(seqs, pad=0):
+    """
+    Converts a set of sequences to a NumPy array of byte-long ASCII codes.
+    """
+    encode_seqs = np.array(
+        [ascii_encode_seq(seq, pad=pad) for seq in seqs], dtype=int
+    )
+    return encode_seqs
+
+
+def ascii_decode_seq(seq):
+    """
+    Converts a NumPy array of byte-long ASCII codes to a string of characters.
+    """
+    return "".join([chr(int(letter)) for letter in seq]).replace("$", "")
+
+
+def ascii_decode_seqs(seqs):
+    """Convert a set of one-hot encoded arrays back to strings"""
+    return np.array(
+        [ascii_decode_seq(seq) for seq in seqs], dtype=object
+    )
+
+
+def reverse_complement_seq(seq, vocab="DNA"):
+    """Reverse complement a single sequence."""
+    if isinstance(seq, str):
+        if vocab == "DNA":
+            return "".join(COMPLEMENT_DNA.get(base, base) for base in reversed(seq))
+        elif vocab == "RNA":
+            return "".join(COMPLEMENT_RNA.get(base, base) for base in reversed(seq))
+        else:
+            raise ValueError("Invalid vocab, only DNA or RNA are currently supported")
+    elif isinstance(seq, np.ndarray):
+        return torch.from_numpy(np.flip(seq, axis=(0, 1)).copy()).numpy()
+
+
+def reverse_complement_seqs(seqs, vocab="DNA", verbose=True):
+    """Reverse complement set of sequences."""
+    if isinstance(seqs[0], str):
+        return np.array(
+            [
+                reverse_complement_seq(seq, vocab)
+                for i, seq in tqdm(
+                    enumerate(seqs),
+                    total=len(seqs),
+                    desc="Reverse complementing sequences",
+                    disable=not verbose,
+                )
+            ]
+        )
+    elif isinstance(seqs[0], np.ndarray):
+        return torch.from_numpy(np.flip(seqs, axis=(1, 2)).copy()).numpy()
+
+
+def ohe_seq(seq, vocab="DNA", neutral_vocab="N", fill_value=0):
+    """Convert a sequence into one-hot-encoded array."""
+    seq = seq.strip().upper()
+    return _token2one_hot(
+        _tokenize(seq, vocab, neutral_vocab), vocab, fill_value=fill_value
+    )
+
+
+def ohe_seqs(
+    seqs,
+    vocab="DNA",
+    neutral_vocab="N",
+    maxlen=None,
+    pad=True,
+    pad_value="N",
+    fill_value=None,
+    seq_align="start",
+    verbose=True,
+):
+    """Convert a set of sequences into one-hot-encoded array."""
+    if isinstance(neutral_vocab, str):
+        neutral_vocab = [neutral_vocab]
+    if isinstance(seqs, str):
+        raise ValueError("seq_vec should be an iterable not a string itself")
+    assert len(vocab[0]) == len(pad_value)
+    assert pad_value in neutral_vocab
+    if pad:
+        seqs_vec = _pad_sequences(seqs, maxlen=maxlen, align=seq_align, value=pad_value)
+    arr_list = [
+        ohe_seq(
+            seq=seqs_vec[i],
+            vocab=vocab,
+            neutral_vocab=neutral_vocab,
+            fill_value=fill_value,
+        )
+        for i in tqdm(
+            range(len(seqs_vec)),
+            total=len(seqs_vec),
+            desc="One-hot encoding sequences",
+            disable=not verbose,
+        )
+    ]
+    if pad:
+        return np.stack(arr_list)
+    else:
+        return np.array(arr_list, dtype=object)
+
+
+def decode_seq(arr, vocab="DNA", neutral_value=-1, neutral_char="N"):
+    """Convert a single one-hot encoded array back to string"""
+    if isinstance(arr, torch.Tensor):
+        arr = arr.numpy()
+    return _sequencize(
+        tvec=_one_hot2token(arr, neutral_value),
+        vocab=vocab,
+        neutral_value=neutral_value,
+        neutral_char=neutral_char,
+    )
+
+
+def decode_seqs(arr, vocab="DNA", neutral_char="N", neutral_value=-1, verbose=True):
+    """Convert a one-hot encoded array back to set of sequences"""
+    arr_list = [
+        decode_seq(
+            arr=arr[i],
+            vocab=vocab,
+            neutral_value=neutral_value,
+            neutral_char=neutral_char,
+        )
+        for i in tqdm(
+            range(len(arr)),
+            total=len(arr),
+            desc="Decoding sequences",
+            disable=not verbose,
+        )
+    ]
+    return np.array(arr_list)
+
+
+def dinuc_shuffle_seq(seq, num_shufs=None, rng=None):
+    """
+    Creates shuffles of the given sequence, in which dinucleotide frequencies
+    are preserved.
+
+    If `seq` is a string, returns a list of N strings of length L, each one
+    being a shuffled version of `seq`. If `seq` is a 2D np array, then the
+    result is an N x L x D np array of shuffled versions of `seq`, also
+    one-hot encoded. If `num_shufs` is not specified, then the first dimension
+    of N will not be present (i.e. a single string will be returned, or an L x D
+    array).
 
     Parameters
     ----------
-    model: torch.nn.Module
-        The model to score the sequences with
-    X: np.ndarray
-        The one-hot encoded sequences to calculate find mutations for.
-    batch_size: int, optional
-        The number of sequences to score at once.
-    device: str, optional
-        Whether to use a 'cpu' or 'cuda'.
+    seq : str
+        The sequence to shuffle.
+    num_shufs : int, optional
+        The number of shuffles to create. If None, only one shuffle is created.
+    rng : np.random.RandomState, optional
+        The random number generator to use. If None, a new one is created.
 
     Returns
     -------
-    mut_X: np.ndarray
-        The highest scoring one-hot-encoded sequences
-    maxs: np.ndarray
-        The highest delta scores corresponding to the highest scoring sequences
-    locs: np.ndarray
-        The indeces along the length of the sequences where the mutations can be found
-
-    """
-    device = "cuda" if settings.gpus > 0 else "cpu" if device is None else device
-    batch_size = settings.batch_size if batch_size is None else batch_size
-    model.eval().to(device)
-    X = X.transpose(0, 2, 1) if X.shape[2] == 4 else X
-    X = torch.Tensor(X).float().numpy()
-    X_ism = _naive_ism(model, X, device=device, batch_size=batch_size)
-    maxs, inds, mut_X = [], [], X.copy()
-    for i in range(len(mut_X)):
-        maxs.append(np.max(X_ism[i]))
-        ind = np.unravel_index(X_ism[i].argmax(), X_ism[i].shape)
-        inds.append(ind[1])
-        mut_X[i][:, ind[1]] = np.zeros(mut_X.shape[1])
-        mut_X[i][:, ind[1]][ind[0]] = 1
-    return mut_X, np.array(maxs), np.array(inds)
-
-
-def evolution(
-    model: torch.nn.Module,
-    X: np.ndarray,
-    rounds: int = 10,
-    k: int = 10,
-    force_different: bool = True,
-    batch_size: int = None,
-    device: str = "cpu",
-) -> np.ndarray:
-    """Perform rounds rounds of in-silico evolution on a single sequence X.
-
-    Using ISM, this function calculates all the scores of all possible mutations
-    on a starting sequence X. It then mutates the sequence and repeats the process
-    for rounds rounds. In the end, it returns new "evolved" sequence after rounds mutations
-    and the delta scores from the reference sequence and the indeces along the lengths of the sequences
-    with which the mutations occured
+    list of str or np.array
+        The shuffled sequences.
 
-    Parameters
-    ----------
-    model: torch.nn.Module
-        The model to score the sequences with
-    X: np.ndarray
-        The one-hot encoded reference sequence to start the evolution with
-    rounds: int, optional
-        The number of rounds of evolution to perform
-    force_different: bool, optional
-        Whether to force the mutations to occur at different locations in the reference sequence
-    k: int, optional
-        The number of mutated sequences to consider at each round. This is in case
-        the same position scores highest multiple times.
-    """
-    device = "cuda" if settings.gpus > 0 else "cpu" if device is None else device
-    batch_size = settings.batch_size if batch_size is None else batch_size
-    model.eval().to(device)
-    curr_X = X.copy()
-    mutated_positions, mutated_scores = [], []
-    for r in range(rounds):
-        mut_X, score, positions = best_k_muts(model, curr_X, k=k, device=device)
-        if force_different:
-            for i, p in enumerate(positions):
-                if p not in mutated_positions:
-                    curr_X = mut_X[i]
-                    mutated_positions.append(p)
-                    mutated_scores.append(score[i])
-                    break
+    Note
+    ----
+    This function comes from DeepLIFT's dinuc_shuffle.py.
+    """
+    if type(seq) is str or type(seq) is np.str_:
+        arr = _string_to_char_array(seq)
+    elif type(seq) is np.ndarray and len(seq.shape) == 2:
+        seq_len, one_hot_dim = seq.shape
+        arr = _one_hot_to_tokens(seq)
+    else:
+        raise ValueError("Expected string or one-hot encoded array")
+    if not rng:
+        rng = np.random.RandomState()
+
+    # Get the set of all characters, and a mapping of which positions have which
+    # characters; use `tokens`, which are integer representations of the
+    # original characters
+    chars, tokens = np.unique(arr, return_inverse=True)
+
+    # For each token, get a list of indices of all the tokens that come after it
+    shuf_next_inds = []
+    for t in range(len(chars)):
+        mask = tokens[:-1] == t  # Excluding last char
+        inds = np.where(mask)[0]
+        shuf_next_inds.append(inds + 1)  # Add 1 for next token
+
+    if type(seq) is str or type(seq) is np.str_:
+        all_results = []
+    else:
+        all_results = np.empty(
+            (num_shufs if num_shufs else 1, seq_len, one_hot_dim), dtype=seq.dtype
+        )
+
+    for i in range(num_shufs if num_shufs else 1):
+        # Shuffle the next indices
+        for t in range(len(chars)):
+            inds = np.arange(len(shuf_next_inds[t]))
+            inds[:-1] = rng.permutation(len(inds) - 1)  # Keep last index same
+            shuf_next_inds[t] = shuf_next_inds[t][inds]
+
+        counters = [0] * len(chars)
+
+        # Build the resulting array
+        ind = 0
+        result = np.empty_like(tokens)
+        result[0] = tokens[ind]
+        for j in range(1, len(tokens)):
+            t = tokens[ind]
+            ind = shuf_next_inds[t][counters[t]]
+            counters[t] += 1
+            result[j] = tokens[ind]
+
+        if type(seq) is str or type(seq) is np.str_:
+            all_results.append(_char_array_to_string(chars[result]))
         else:
-            curr_X = mut_X[0]
-            mutated_positions.append(positions[0])
-            mutated_scores.append(score[0])
-    return curr_X, mutated_scores, mutated_positions
+            all_results[i] = _tokens_to_one_hot(chars[result], one_hot_dim)
+    return all_results if num_shufs else all_results[0]
 
 
-@track
-def evolve_seqs_sdata(
-    model: torch.nn.Module, 
-    sdata, 
-    rounds: int, 
-    return_seqs: bool = False, 
-    device: str = "cpu", 
-    copy: bool = False, 
-    **kwargs
-):
+def dinuc_shuffle_seqs(seqs, num_shufs=None, rng=None):
     """
-    In silico evolve a set of sequences that are stored in a SeqData object.
+    Shuffle the sequences in `seqs` in the same way as `dinuc_shuffle_seq`.
+    If `num_shufs` is not specified, then the first dimension of N will not be
+    present (i.e. a single string will be returned, or an L x D array).
 
     Parameters
     ----------
-    model: torch.nn.Module  
-        The model to score the sequences with
-    sdata: SeqData  
-        The SeqData object containing the sequences to evolve
-    rounds: int
-        The number of rounds of evolution to perform
-    return_seqs: bool, optional
-        Whether to return the evolved sequences
-    device: str, optional
-        Whether to use a 'cpu' or 'cuda'.
-    copy: bool, optional
-        Whether to copy the SeqData object before mutating it
-    kwargs: dict, optional
-        Additional arguments to pass to the evolution function
-    
+    seqs : np.ndarray
+        Array of sequences to shuffle
+    num_shufs : int, optional
+        Number of shuffles to create, by default None
+    rng : np.random.RandomState, optional
+        Random state to use for shuffling, by default None
+
     Returns
     -------
-    sdata: SeqData
-        The SeqData object containing the evolved sequences
+    np.ndarray
+        Array of shuffled sequences
+
+    Note
+    -------
+    This is taken from DeepLIFT
     """
-    sdata = sdata.copy() if copy else sdata
-    device = "cuda" if settings.gpus > 0 else "cpu" if device is None else device
-    model.eval().to(device)
-    evolved_seqs = np.zeros(sdata.ohe_seqs.shape)
-    deltas = np.zeros((sdata.n_obs, rounds))
-    for i, ohe_seq in tqdm(enumerate(sdata.ohe_seqs), total=len(sdata.ohe_seqs), desc="Evolving seqs"):
-        evolved_seq, delta, _ = evolution(model, ohe_seq, rounds=rounds, device=device)
-        evolved_seqs[i] = evolved_seq
-        deltas[i, :] = deltas[i, :] + delta
-    orig_seqs = torch.Tensor(sdata.ohe_seqs).to(device)
-    original_scores = model(orig_seqs).detach().cpu().numpy().squeeze()
-    sdata["original_score"] = original_scores
-    sdata["evolved_1_score"] = original_scores + deltas[:, 0]
-    for i in range(2, rounds + 1):
-        sdata.seqs_annot[f"evolved_{i}_score"] = (
-            sdata.seqs_annot[f"evolved_{i-1}_score"] + deltas[:, i - 1]
-        )
-    print(return_seqs)
-    if return_seqs:
-        evolved_seqs = torch.Tensor(evolved_seqs).to(device)
-        return evolved_seqs
-    return sdata if copy else None
-
-
-def feature_implant_seq_sdata(
-    model: torch.nn.Module,
-    sdata,
-    seq_id: str,
-    feature: np.ndarray,
-    feature_name: str = "feature",
-    encoding: str = "str",
-    onehot: bool = False,
-    store: bool = True,
-    device: str = "cpu",
-):
+    if not rng:
+        rng = np.random.RandomState()
+
+    if type(seqs) is str or type(seqs) is np.str_:
+        seqs = [seqs]
+
+    all_results = []
+    for i in range(len(seqs)):
+        all_results.append(dinuc_shuffle_seq(seqs[i], num_shufs=num_shufs, rng=rng))
+    return np.array(all_results)
+
+
+def perturb_seq(X_0, vocab_len=4):
+    """
+    Produce all edit-distance-one pertuabtions for a single of sequences.
+
+    Note
+    ----
+    This function is modified from the Yuzu package
+    """
+    import warnings
+
+    if not isinstance(X_0, np.ndarray):
+        raise ValueError("X_0 must be of type np.ndarray, not {}".format(type(X_0)))
+
+    if len(X_0.shape) != 2:
+        raise ValueError("X_0 must have two dimensions: (n_choices, seq_len).")
+
+    if X_0.shape[0] != 4:
+        warnings.warn(
+            "X_0 has {} choices, but should have 4. Transposing".format(X_0.shape[1])
+        )
+        X_0 = X_0.transpose()
+
+    n_choices, seq_len = X_0.shape
+    idx = X_0.argmax(axis=0)
+    X_0 = torch.from_numpy(X_0)
+
+    n = seq_len * (n_choices - 1)
+    X = torch.tile(X_0, (n, 1))
+    X = X.reshape(n, n_choices, seq_len)
+    for k in range(1, n_choices):
+        i = np.arange(seq_len) * (n_choices - 1) + (k - 1)
+        X[i, idx, np.arange(seq_len)] = 0
+        X[i, (idx + k) % n_choices, np.arange(seq_len)] = 1
+
+    return X.numpy()
+
+
+def perturb_seqs(X_0, vocab_len=4):
     """
-    Score a set of sequences with a feature inserted at every position of each sequence in sdata.
-    For double stranded models, the feature is inserted in both strands, with the reverse complement
-    of the feature in the reverse strand
+    Produce all edit-distance-one pertuabtions for a set of sequences.
+
+    This function will take in a single one-hot encoded sequence of length N
+    and return a batch of N*(n_choices-1) sequences, each containing a single
+    perturbation from the given sequence.
 
     Parameters
     ----------
-    model: torch.nn.Module
-        The model to score the sequences with
-    sdata: SeqData
-        The SeqData object containing the sequences to score
-    seq_id: str
-        The id of the sequence to score
-    feature: np.ndarray
-        The feature to insert into the sequences
-    feature_name: str, optional
-        The name of the feature
-    encoding: str, optional
-        The encoding of the feature. One of 'str', 'ohe', 'int'
-    onehot: bool, optional
-        Whether the feature is one-hot encoded
-    store: bool, optional
-        Whether to store the scores in the SeqData object
-    device: str, optional
-        Whether to use a 'cpu' or 'cuda'.
+    X_0: np.ndarray, shape=(n_seqs, n_choices, seq_len)
+        A one-hot encoded sequence to generate all potential perturbations.
 
     Returns
     -------
-    np.ndarray
-        The scores of the sequences with the feature inserted if store is False
+    X: torch.Tensor, shape=(n_seqs, (n_choices-1)*seq_len, n_choices, seq_len)
+        Each single-position perturbation of seq.
+
+    Note
+    ----
+    This function is modified from the Yuzu package.
+    """
+    import warnings
+
+    if not isinstance(X_0, np.ndarray):
+        raise ValueError("X_0 must be of type np.ndarray, not {}".format(type(X_0)))
+
+    if len(X_0.shape) != 3:
+        raise ValueError(
+            "X_0 must have three dimensions: (n_seqs, n_choices, seq_len)."
+        )
+    if X_0.shape[1] != 4:
+        warnings.warn(
+            "X_0 has {} choices, but should have 4. Transposing".format(X_0.shape[1])
+        )
+        X_0 = X_0.transpose(0, 2, 1)
+
+    n_seqs, n_choices, seq_len = X_0.shape
+    idxs = X_0.argmax(axis=1)
+
+    X_0 = torch.from_numpy(X_0)
+
+    n = seq_len * (n_choices - 1)
+    X = torch.tile(X_0, (n, 1, 1))
+
+    X = X.reshape(n, n_seqs, n_choices, seq_len).permute(1, 0, 2, 3)
+
+    for i in range(n_seqs):
+        for k in range(1, n_choices):
+            idx = np.arange(seq_len) * (n_choices - 1) + (k - 1)
+
+            X[i, idx, idxs[i], np.arange(seq_len)] = 0
+            X[i, idx, (idxs[i] + k) % n_choices, np.arange(seq_len)] = 1
+
+    return X
+
+
+def feature_implant_seq(
+    seq, feature, position, vocab="DNA", encoding="str", onehot=False
+):
+    """
+    Insert a feature at a given position in a single sequence.
     """
-    device = "cuda" if settings.gpus > 0 else "cpu" if device is None else device
-    model.eval().to(device)
-    seq_idx = np.where(sdata.seqs_annot.index == seq_id)[0][0]
     if encoding == "str":
-        seq = sdata.seqs[seq_idx]
-        implanted_seqs = feature_implant_across_seq(seq, feature, encoding=encoding)
-        implanted_seqs = ohe_seqs(implanted_seqs, vocab="DNA", verbose=False)
-        X = torch.from_numpy(implanted_seqs).float()
+        return seq[:position] + feature + seq[position + len(feature) :]
     elif encoding == "onehot":
-        seq = sdata.ohe_seqs[seq_idx]
-        implanted_seqs = feature_implant_across_seq(
-            seq, 
-            feature, 
-            encoding=encoding, 
-            onehot=onehot
+        if onehot:
+            feature = _token2one_hot(feature.argmax(axis=1), vocab=vocab, fill_value=0)
+        if feature.shape[0] != seq.shape[0]:
+            feature = feature.transpose()
+        return np.concatenate(
+            (seq[:, :position], feature, seq[:, position + feature.shape[-1] :]), axis=1
         )
-        X = torch.from_numpy(implanted_seqs).float()
     else:
         raise ValueError("Encoding not recognized.")
-    if model.strand == "ss":
-        X = X.to(device)
-        X_rev = X
-    else:
-        X = X.to(device)
-        X_rev = torch.flip(X, [1, 2]).to(device)
-    preds = model(X, X_rev).cpu().detach().numpy().squeeze()
-    if store:
-        sdata.seqsm[f"{seq_id}_{feature_name}_slide"] = preds
-    return preds
 
 
-def feature_implant_seqs_sdata(
-    model: torch.nn.Module,
-    sdata,
-    feature: np.ndarray,
-    seqsm_key: str = None, 
-    device: str = "cpu",
-    **kwargs
-):
+def feature_implant_across_seq(seq, feature, **kwargs):
     """
-    Score a set of sequences with a feature inserted at every position of each sequence in sdata
+    Insert a feature at every position for a single sequence.
+    """
+    if isinstance(seq, str):
+        assert isinstance(feature, str)
+        seq_len = len(seq)
+        feature_len = len(feature)
+    elif isinstance(seq, np.ndarray):
+        assert isinstance(feature, np.ndarray)
+        seq_len = seq.shape[-1]
+        if feature.shape[0] != seq.shape[0]:
+            feature_len = feature.shape[0]
+        else:
+            feature_len = feature.shape[-1]
+    implanted_seqs = []
+    for pos in range(seq_len - feature_len + 1):
+        seq_implanted = feature_implant_seq(seq, feature, pos, **kwargs)
+        implanted_seqs.append(seq_implanted)
+    return np.array(implanted_seqs)
 
-    Parameters
-    ----------
-    model: torch.nn.Module
-        The model to score the sequences with
-    sdata: SeqData
-        The SeqData object containing the sequences to score
-    feature: np.ndarray
-        The feature to insert into the sequences
-    seqsm_key: str, optional
-        The key to store the scores in the SeqData object
-    kwargs: dict, optional
-        Additional arguments to pass to the feature_implant_seq_sdata function
+
+def gc_content_seq(seq, ohe=False):
+    if ohe:
+        return np.sum(seq[1:3, :])/seq.shape[1]
+    else:
+        return (seq.count("G") + seq.count("C"))/len(seq)
     
-    Returns
-    -------
-    np.ndarray
-        The scores of the sequences with the feature inserted if seqsm_key is None
-    """
-    device = "cuda" if settings.gpus > 0 else "cpu" if device is None else device
-    model.eval().to(device)
-    predictions = []
-    for i, seq_id in tqdm(
-        enumerate(sdata.seqs_annot.index),
-        desc="Implanting feature in all seqs of sdata",
-        total=len(sdata.seqs_annot),
-    ):
-        predictions.append(
-            feature_implant_seq_sdata(
-                model, 
-                sdata, 
-                seq_id, 
-                feature, 
-                store=False, 
-                **kwargs
-            )
-        )
-    if seqsm_key is not None:
-        sdata.seqsm[seqsm_key] = np.array(predictions)
+    
+def gc_content_seqs(seqs, ohe=False):
+    if ohe:
+        seq_len = seqs[0].shape[1]
+        return np.sum(seqs[:, 1:3, :], axis=1).sum(axis=1)/seq_len
     else:
-        return np.array(predictions)
+        return np.array([gc_content_seq(seq) for seq in seqs])
+
```

