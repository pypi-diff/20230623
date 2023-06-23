# Comparing `tmp/seqpro-0.0.1.tar.gz` & `tmp/seqpro-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqpro-0.0.1.tar", max compression
+gzip compressed data, was "seqpro-0.1.0.tar", max compression
```

## Comparing `seqpro-0.0.1.tar` & `seqpro-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,21 @@
--rw-r--r--   0        0        0      355 2023-03-26 17:30:44.000000 seqpro-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      567 2023-03-26 17:21:33.000000 seqpro-0.0.1/seqpro/__init__.py
--rw-r--r--   0        0        0     1793 2023-03-26 17:21:38.000000 seqpro-0.0.1/seqpro/_analyzers.py
--rw-r--r--   0        0        0      421 2023-03-26 17:05:22.000000 seqpro-0.0.1/seqpro/_cleaners.py
--rw-r--r--   0        0        0     4707 2023-03-26 17:17:52.000000 seqpro-0.0.1/seqpro/_encoders.py
--rw-r--r--   0        0        0     6560 2023-03-26 17:12:13.000000 seqpro-0.0.1/seqpro/_experimental.py
--rw-r--r--   0        0        0     9445 2023-03-26 17:13:53.000000 seqpro-0.0.1/seqpro/_helpers.py
--rw-r--r--   0        0        0     4762 2023-03-26 17:19:35.000000 seqpro-0.0.1/seqpro/_modifiers.py
--rw-r--r--   0        0        0      626 2023-03-26 17:32:29.707900 seqpro-0.0.1/setup.py
--rw-r--r--   0        0        0      505 2023-03-26 17:32:29.708152 seqpro-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      520 2023-06-23 17:13:31.000000 seqpro-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      977 2023-06-23 16:04:56.000000 seqpro-0.1.0/seqpro/__init__.py
+-rw-r--r--   0        0        0     5455 2023-06-11 21:58:41.000000 seqpro-0.1.0/seqpro/_analyzers.py
+-rw-r--r--   0        0        0     1276 2023-06-01 00:42:03.000000 seqpro-0.1.0/seqpro/_cleaners.py
+-rw-r--r--   0        0        0        0 2023-03-30 18:14:39.000000 seqpro-0.1.0/seqpro/_comparisons.py
+-rw-r--r--   0        0        0     5098 2023-06-23 16:45:31.000000 seqpro-0.1.0/seqpro/_encoders.py
+-rw-r--r--   0        0        0     6782 2023-06-21 17:46:41.000000 seqpro-0.1.0/seqpro/_modifiers.py
+-rw-r--r--   0        0        0     3535 2023-06-21 17:46:41.000000 seqpro-0.1.0/seqpro/_numba.py
+-rw-r--r--   0        0        0     3810 2023-06-23 16:04:56.000000 seqpro-0.1.0/seqpro/_utils.py
+-rw-r--r--   0        0        0     1458 2023-06-11 21:58:41.000000 seqpro-0.1.0/seqpro/alphabets/__init__.py
+-rw-r--r--   0        0        0     8278 2023-06-21 17:46:41.000000 seqpro-0.1.0/seqpro/alphabets/_alphabets.py
+-rw-r--r--   0        0        0     2504 2023-06-23 17:05:29.000000 seqpro-0.1.0/seqpro/deprecated/_analyzers.py
+-rw-r--r--   0        0        0     1358 2023-06-23 17:05:27.000000 seqpro-0.1.0/seqpro/deprecated/_cleaners.py
+-rw-r--r--   0        0        0     4364 2023-06-23 17:05:11.000000 seqpro-0.1.0/seqpro/deprecated/_encoders.py
+-rw-r--r--   0        0        0     9481 2023-06-23 16:48:35.000000 seqpro-0.1.0/seqpro/deprecated/_helpers.py
+-rw-r--r--   0        0        0     6113 2023-06-23 17:05:21.000000 seqpro-0.1.0/seqpro/deprecated/_modifiers.py
+-rw-r--r--   0        0        0     1419 2023-06-23 17:05:25.000000 seqpro-0.1.0/seqpro/deprecated/_utils.py
+-rw-r--r--   0        0        0     2162 2023-06-23 17:05:59.000000 seqpro-0.1.0/seqpro/experimental/_experimental.py
+-rw-r--r--   0        0        0      773 2023-06-23 17:05:39.000000 seqpro-0.1.0/seqpro/experimental/_visualizers.py
+-rw-r--r--   0        0        0     6198 2023-06-21 17:46:41.000000 seqpro-0.1.0/seqpro/xr/__init__.py
+-rw-r--r--   0        0        0      622 1970-01-01 00:00:00.000000 seqpro-0.1.0/PKG-INFO
```

### Comparing `seqpro-0.0.1/seqpro/_analyzers.py` & `seqpro-0.1.0/seqpro/deprecated/_analyzers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,72 @@
 import numpy as np
-np.random.seed(13)
+
+
+# my own
+def len_seqs(seqs, ohe=False):
+    """Calculate the length of each sequence in a list.
+    
+    Parameters
+    ----------
+    seqs : list
+        List of sequences.
+    ohe : bool, optional
+        Whether to calculate the length of one-hot encoded sequences.
+        Default is False.
+        
+    Returns
+    -------
+    np.array
+        Array containing the length of each sequence.
+    """
+    if ohe:
+        return np.array([seq.shape[1] for seq in seqs])
+    else:
+        return np.array([len(seq) for seq in seqs])
 
 # my own
-def gc_content_seq(seq, ohe=True):
+def gc_content_seq(seq, ohe=False):
     if ohe:
         return np.sum(seq[1:3, :])/seq.shape[1]
     else:
         return (seq.count("G") + seq.count("C"))/len(seq)
 
 # my own
-def gc_content_seqs(seqs, ohe=True):
+def gc_content_seqs(seqs, ohe=False):
     if ohe:
         seq_len = seqs[0].shape[1]
         return np.sum(seqs[:, 1:3, :], axis=1).sum(axis=1)/seq_len
     else:
         return np.array([gc_content_seq(seq) for seq in seqs])
 
 # my own
-def nucleotide_content_seq(seq, ohe=True, normalize=True):
+def nucleotide_content_seq(seq, ohe=False, normalize=True):
     if ohe:
         if normalize:
             return np.sum(seq, axis=1)/seq.shape[1]
         else:
             return np.sum(seq, axis=1)
     else:
         if normalize:
             return np.array([seq.count(nuc)/len(seq) for nuc in "ACGT"])
         else:
             return np.array([seq.count(nuc) for nuc in "ACGT"])
             
 # my own
-def nucleotide_content_seqs(seqs, axis=0, ohe=True, normalize=True):
+def nucleotide_content_seqs(seqs, axis=0, ohe=False, normalize=True):
     if ohe:
         if normalize:
             return np.sum(seqs, axis=axis)/seqs.shape[0]
         else:
             return np.sum(seqs, axis=axis)
     else:
-        print("Not implemented yet")
+        if normalize:
+            return np.array([np.array([seq.count(nuc)/len(seq) for nuc in "ACGT"]) for seq in seqs])
+        else:
+            return np.array([np.array([seq.count(nuc) for nuc in "ACGT"]) for seq in seqs])
 
 # haydens
 def count_kmers_seq(seq : str, k : int, data = None) -> dict:
     """
     Counts k-mers in a given seq.
     Parameters
     ----------
@@ -58,8 +83,8 @@
     data = {} if data is None else data
     for i in range(len(seq) - k + 1):
         kmer = seq[i: i + k]
         try:
             data[kmer] += 1
         except KeyError:
             data[kmer] = 1
-    return data
+    return data
```

### Comparing `seqpro-0.0.1/seqpro/_encoders.py` & `seqpro-0.1.0/seqpro/deprecated/_encoders.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,100 +1,89 @@
 import torch
 import numpy as np
-np.random.seed(13)
 from tqdm.auto import tqdm
-from ._helpers import DNA, RNA, COMPLEMENT_DNA, COMPLEMENT_RNA
-from ._helpers import _token2one_hot, _tokenize, _pad_sequences, _sequencize, _one_hot2token
+from typing import List, Union, Optional, Iterable
+from _helpers import _token2one_hot, _tokenize, _pad_sequences, _sequencize, _one_hot2token, _one_hot2token, _token2one_hot
+
 
 # my own
-def ascii_encode_seq(seq, pad=0):
+def ascii_encode_seq(seq: str, pad: int = 0) -> np.array:
     """
     Converts a string of characters to a NumPy array of byte-long ASCII codes.
+
+    Parameters
+    ----------
+    seq : str
+        Sequence to encode.
+    pad : int
+        Amount of padding to add to the end of the sequence. Defaults to 0.
+
+    Returns
+    -------
     """
     encode_seq = np.array([ord(letter) for letter in seq], dtype=int)
     if pad > 0:
         encode_seq = np.pad(encode_seq, pad_width=(0, pad), mode="constant", constant_values=36)
     return encode_seq
 
 # my own
-def ascii_encode_seqs(seqs, pad=0):
+def ascii_encode_seqs(seqs: List[str], pad: int = 0) -> np.ndarray:
     """
     Converts a set of sequences to a NumPy array of byte-long ASCII codes.
+
+    Parameters
+    ----------
+    seqs : List[str]
+        Sequences to encode.
+    pad : int
+        Amount of padding to add to the end of the sequences. Defaults to 0.
+    
+    Returns
+    -------
+    np.ndarray
+        Array of encoded sequences.
     """
-    encode_seqs = np.array(
-        [ascii_encode_seq(seq, pad=pad) for seq in seqs], dtype=int
-    )
+    encode_seqs = np.array([ascii_encode_seq(seq, pad=pad) for seq in seqs], dtype=int)
     return encode_seqs
 
 # my own
-def ascii_decode_seq(seq):
+def ascii_decode_seq(seq: np.array) -> str:
     """
     Converts a NumPy array of byte-long ASCII codes to a string of characters.
     """
     return "".join([chr(int(letter)) for letter in seq]).replace("$", "")
 
 # my own
-def ascii_decode_seqs(seqs):
+def ascii_decode_seqs(seqs: np.ndarray) -> np.array:
     """Convert a set of one-hot encoded arrays back to strings"""
     return np.array([ascii_decode_seq(seq) for seq in seqs], dtype=object)
 
-# my own
-def reverse_complement_seq(seq, vocab="DNA"):
-    """Reverse complement a single sequence."""
-    if isinstance(seq, str):
-        if vocab == "DNA":
-            return "".join(COMPLEMENT_DNA.get(base, base) for base in reversed(seq))
-        elif vocab == "RNA":
-            return "".join(COMPLEMENT_RNA.get(base, base) for base in reversed(seq))
-        else:
-            raise ValueError("Invalid vocab, only DNA or RNA are currently supported")
-    elif isinstance(seq, np.ndarray):
-        return torch.from_numpy(np.flip(seq, axis=(0, 1)).copy()).numpy()
-
-# my own
-def reverse_complement_seqs(seqs, vocab="DNA", verbose=True):
-    """Reverse complement set of sequences."""
-    if isinstance(seqs[0], str):
-        return np.array(
-            [
-                reverse_complement_seq(seq, vocab)
-                for i, seq in tqdm(
-                    enumerate(seqs),
-                    total=len(seqs),
-                    desc="Reverse complementing sequences",
-                    disable=not verbose,
-                )
-            ]
-        )
-    elif isinstance(seqs[0], np.ndarray):
-        return torch.from_numpy(np.flip(seqs, axis=(1, 2)).copy()).numpy()
-
 # modifed concise
 def ohe_seq(
-    seq, 
-    vocab="DNA", 
-    neutral_vocab="N", 
-    fill_value=0
-):
+    seq: str, 
+    vocab: str = "DNA", 
+    neutral_vocab: str = "N", 
+    fill_value: int = 0
+) -> np.array:
     """Convert a sequence into one-hot-encoded array."""
     seq = seq.strip().upper()
     return _token2one_hot(_tokenize(seq, vocab, neutral_vocab), vocab, fill_value=fill_value)
 
 # modfied concise
 def ohe_seqs(
-    seqs,
-    vocab="DNA",
-    neutral_vocab="N",
-    maxlen=None,
-    pad=True,
-    pad_value="N",
-    fill_value=None,
-    seq_align="start",
-    verbose=True,
-):
+    seqs: Iterable[str],
+    vocab: str = "DNA",
+    neutral_vocab: Union[str, List[str]] = "N",
+    maxlen: Optional[int] = None,
+    pad: bool = True,
+    pad_value: str = "N",
+    fill_value: Optional[str] = None,
+    seq_align: str = "start",
+    verbose: bool = True,
+) -> np.ndarray:
     """Convert a set of sequences into one-hot-encoded array."""
     if isinstance(neutral_vocab, str):
         neutral_vocab = [neutral_vocab]
     if isinstance(seqs, str):
         raise ValueError("seq_vec should be an iterable not a string itself")
     assert len(vocab[0]) == len(pad_value)
     assert pad_value in neutral_vocab
@@ -116,36 +105,48 @@
     ]
     if pad:
         return np.stack(arr_list)
     else:
         return np.array(arr_list, dtype=object)
 
 # my own
-def decode_seq(arr, vocab="DNA", neutral_value=-1, neutral_char="N"):
+def decode_seq(
+    arr: np.ndarray,
+    vocab: str = "DNA",
+    neutral_value: int = -1,
+    neutral_char: str = "N"
+) -> str:
     """Convert a single one-hot encoded array back to string"""
     if isinstance(arr, torch.Tensor):
         arr = arr.numpy()
     return _sequencize(
         tvec=_one_hot2token(arr, neutral_value),
         vocab=vocab,
         neutral_value=neutral_value,
         neutral_char=neutral_char,
     )
 
 # my own
-def decode_seqs(arr, vocab="DNA", neutral_char="N", neutral_value=-1, verbose=True):
+def decode_seqs(
+    arr: np.ndarray,
+    vocab: str = "DNA",
+    neutral_char: str = "N",
+    neutral_value: int = -1,
+    verbose: bool = True
+) -> np.ndarray:
     """Convert a one-hot encoded array back to set of sequences"""
-    arr_list = [
+    arr_list: List[np.ndarray] = [
         decode_seq(
             arr=arr[i],
             vocab=vocab,
             neutral_value=neutral_value,
             neutral_char=neutral_char,
         )
         for i in tqdm(
             range(len(arr)),
             total=len(arr),
             desc="Decoding sequences",
             disable=not verbose,
         )
     ]
     return np.array(arr_list)
+
```

### Comparing `seqpro-0.0.1/seqpro/_experimental.py` & `seqpro-0.1.0/seqpro/_modifiers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,209 +1,226 @@
-import torch
+from typing import Optional, Tuple, Union, cast
+
 import numpy as np
-np.random.seed(13)
-from seqdata import SeqData
-from ._encoders import decode_seq
-from ._analyzers import count_kmers
-from ._helpers import _token2one_hot
+import ushuffle
+from numpy.typing import NDArray
 
+from ._numba import gufunc_jitter_helper
+from ._utils import SeqType, _check_axes, cast_seqs
+from .alphabets._alphabets import NucleotideAlphabet
 
-# EUGENe on sdata
-def count_kmers_sdata(sdata : SeqData, k : int, frequency : bool = False) -> dict:
-    """
-    Counts k-mers in a given sequence from a SeqData object.
+
+def reverse_complement(
+    seqs: SeqType,
+    alphabet: NucleotideAlphabet,
+    length_axis: Optional[int] = None,
+    ohe_axis: Optional[int] = None,
+):
+    """Reverse complement a sequence.
 
     Parameters
     ----------
-    sdata : SeqData
-        SeqData object containing sequences.
-    k : int
-        k value for k-mers (e.g. k=3 generates 3-mers).
-    frequency : bool
-        Whether to return relative k-mer frequency in place of count.
-        Default is False.
+    seqs : str, list[str], ndarray[str, bytes, uint8]
+    alphabet : NucleotideAlphabet
+    length_axis : Optional[int], optional
+        Needed for array input. Length axis, by default None
+    ohe_axis : Optional[int], optional
+        Needed for OHE input. One hot encoding axis, by default None
 
     Returns
     -------
-    kmers : dict
-        k-mers and their counts expressed in a dictionary.
+    ndarray[bytes, uint8]
+        Array of bytes (S1) or uint8 for string or OHE input, respectively.
     """
-    data = {}
-    for seq in sdata.seqs:
-        data = count_kmers(seq, k, data)
-    if frequency:
-        total = sum(data.values())
-        for kmer in data:
-            data[kmer] = data[kmer] / total
-    return data
-
-# helper
-def _find_distance(seq1, seq2) -> int:
-    edits = 0
-    for i in range(len(seq1)):
-        if seq1[i] != seq2[i]:
-            edits += 1
-    return edits
+    return alphabet.reverse_complement(seqs, length_axis, ohe_axis)
 
-# analyzers?
-def edit_distance(seq1 : str, seq2 : str, dual : bool = False) -> int:
-    """
-    Calculates the nucleotide edit distance between two sequences.
+
+def k_shuffle(
+    seqs: SeqType,
+    k: int,
+    *,
+    length_axis: Optional[int] = None,
+    ohe_axis: Optional[int] = None,
+    seed: Optional[int] = None,
+    alphabet: Optional[NucleotideAlphabet] = None,
+) -> NDArray[Union[np.bytes_, np.uint8]]:
+    """Shuffle sequences while preserving k-let frequencies.
 
     Parameters
     ----------
-    seq1 : str
-        First nucleotide sequence expressed as a string.
-    seq2 : str
-        Second ucleotide sequence expressed as a string.
-    dual : bool
-        Whether to calculate the forwards and backwards edit distance, and return the lesser.
-        Defaults to False.
+    seqs : SeqType
+    k : int
+        Size of k-lets to preserve frequencies of.
+    length_axis : Optional[int], optional
+        Needed for array input. Axis that corresponds to the length of sequences.
+    ohe_axes : Optional[int], optional
+        Needed for OHE input. Axis that corresponds to the one hot encoding, should be
+        the same size as the length of the alphabet.
+    seed : Optional[int], optional
+        Seed for shuffling.
+    alphabet : Optional[NucleotideAlphabet], optional
+        Alphabet, needed for OHE sequence input.
+    """
+
+    _check_axes(seqs, length_axis, ohe_axis)
+
+    seqs = cast_seqs(seqs)
+
+    # only get here if seqs was str or list[str]
+    if length_axis is None:
+        length_axis = -1
+
+    if k == 1:
+        rng = np.random.default_rng(seed)
+        return rng.permuted(seqs, axis=length_axis)
+
+    if seed is not None:
+        import importlib
+
+        importlib.reload(ushuffle)
+        ushuffle.set_seed(seed)
+
+    seqs = seqs.copy()
+
+    if seqs.dtype == np.uint8:
+        assert ohe_axis is not None
+        seqs = cast(NDArray[np.uint8], seqs)
+        ohe = True
+        if alphabet is None:
+            raise ValueError("Need an alphabet to process OHE sequences.")
+        seqs = alphabet.decode_ohe(seqs, ohe_axis=ohe_axis)
+    else:
+        ohe = False
 
-    Returns
-    -------
-    edits : int
-        Amount of edits between sequences.
-    """
-    assert len(seq1) == len(seq2), "Both sequences must be of same length."
-    f_edits = _find_distance(seq1, seq2)
-    b_edits = _find_distance(seq1, seq2[::-1]) if dual else len(seq1)
-    return min(f_edits, b_edits)
+    length = seqs.shape[length_axis]
+    with np.nditer(
+        seqs.view(f"S{length}").ravel(), op_flags=["readwrite"]  # type: ignore
+    ) as it:
+        for seq in it:
+            seq[...] = ushuffle.shuffle(seq.tobytes(), k)  # type: ignore
+
+    if ohe:
+        assert ohe_axis is not None
+        assert alphabet is not None
+        seqs = cast(NDArray[np.bytes_], seqs)
+        seqs = alphabet.ohe(seqs).swapaxes(-1, ohe_axis)
+
+    return seqs
 
-# EUGENe on sdata?
-def edit_distance_sdata(sdata1 : SeqData, sdata2 : SeqData, dual : bool = False, average : bool = False) -> list:
-    """
-    Calculates the nucleotide edit distance between pairs of sequences from a SeqData object.
+
+def bin_coverage(
+    coverage: NDArray[np.number],
+    bin_width: int,
+    length_axis: int,
+    normalize=False,
+) -> NDArray[np.number]:
+    """Bin coverage by summing over non-overlapping windows.
 
     Parameters
     ----------
-    sdata1 : SeqData
-        First SeqData object containing sequences.
-    sdata2 : SeqData
-        Second SeqData object containing sequences.
-    dual : bool
-        Whether to calculate the forwards and backwards edit distance, and return the lesser.
-        Defaults to False.
-    average : bool
-        Whether to average all edit distances and return in place of a list.
-        Defaults to False.
+    coverage_array : NDArray
+    bin_width : int
+        Width of the windows to sum over. Must be an even divisor of the length
+        of the coverage array. If not, raises an error. The length dimension is
+        assumed to be the second dimension.
+    length_axis: int
+    normalize : bool, default False
+        Whether to normalize by the length of the bin.
 
     Returns
     -------
-    edits : list
-        List containing itemized amounts of edits between sequences.
+    binned_coverage : NDArray
     """
-    assert len(sdata1.seqs) == len(sdata2.seqs), "Both SeqData objects must be of the same length."
-    distances = []
-    for i in range(len(sdata1.seqs)):
-        distances.append(edit_distance(sdata1.seqs[i], sdata2.seqs[i], dual))
-    if average:
-        return sum(distances) / len(distances)
-    return distances
+    length = coverage.shape[length_axis]
+    if length % bin_width != 0:
+        raise ValueError("Bin width must evenly divide length.")
+    binned_coverage = np.add.reduceat(
+        coverage, np.arange(0, length, bin_width), axis=length_axis
+    )
+    if normalize:
+        binned_coverage /= bin_width
+    return binned_coverage
 
-# EUGENe for generative models
-def latent_interpolation(latent_dim : int, samples : int, num_seqs : int = 1, generator = None, normal : bool = False, inclusive : bool = True) -> list:
-    """
-    Linearly interpolates between two random latent points. Useful for visualizing generative generators.
+
+def jitter(
+    *arrays: NDArray,
+    max_jitter: int,
+    length_axis: int,
+    jitter_axes: Union[int, Tuple[int, ...]],
+    seed: Optional[int] = None,
+):
+    """Randomly jitter data from arrays, using the same jitter across arrays.
 
     Parameters
     ----------
-    latent_dim : int
-        Latent dimension of random latent space points.
-    samples : int
-        Number of samples to make between the two latent points. Higher numbers represent more sequences and should show smoother results.
-    num_seqs : int
-        Number of sequence channels to interpolate.
-        Defaults to 1.
-    generator : Basgeneratore
-        If provided, interpolated values will be passed through the given generator and be returned in place of latent points.
-        Default is None.
-    normal : bool
-        Whether to randomly sample points from a standard normal distibution rather than from 0 to 1.
-        Defaults to False.
-    inclusive : bool
-        Whether to returm random latent points along with their interpolated samples.
-        Defaults to True.
+    *arrays : NDArray
+        Arrays to be jittered. They must have the same sizez jitter and length
+        axes.
+    max_jitter : int
+        Maximum jitter amount.
+    length_axis : int
+    jitter_axes : Tuple[int, ...]
+        Each element along the jitter axes will be randomly jittered *independently*.
+        Thus, if jitter_axes = 0, then every slice of data along axis 0 would be
+        jittered independently. If jitter_axes = (0, 1), then each element along axes 0
+        and 1 would be randomly jittered independently.
+    seed : Optional[int], optional
+        Random seed, by default None
 
     Returns
     -------
-    z_list : list
-        List of latent space points represented as tensors.
-    gen_seqs : list
-        List of tokenized sequences expressed as strings.
-        Returns in place of z_list when a generator is provided.
+    arrays
+        Jittered arrays. Will have a new length equal to length - 2*max_jitter.
     """
-    if normal:
-        z1 = torch.normal(0, 1, (num_seqs, latent_dim))
-        z2 = torch.normal(0, 1, (num_seqs, latent_dim))
-    else:
-        z1 = torch.rand(num_seqs, latent_dim)
-        z2 = torch.rand(num_seqs, latent_dim)
+    if isinstance(jitter_axes, int):
+        jitter_axes = (jitter_axes,)
 
-    z_list = []
-    for n in range(samples):
-        weight = (n + 1)/(samples + 1)
-        z_interp = torch.lerp(z1, z2, weight)
-        z_list.append(z_interp)
-    if inclusive:
-        z_list.insert(0, z1)
-        z_list.append(z2)
-
-    if generator is None:
-        return z_list
-
-    gen_seqs = []
-    for z in z_list:
-        gen_seq = seqs_from_tensor(generator(z))
-        gen_seqs.append(gen_seq)
-    return gen_seqs
+    destination_axes = list(range(-len(jitter_axes) - 1, 0))
+    arrays = [
+        np.moveaxis(a, [*jitter_axes, length_axis], destination_axes) for a in arrays
+    ]
 
-# helper?
-def seqs_from_tensor(tensor : torch.tensor, num_seqs : int = 1) -> np.ndarray:
-    """
-    Decodes sequences represented by tensors into their string values.
+    jitter_axes_shape = arrays[0].shape[-len(destination_axes) : -1]
+    for arr in arrays:
+        if arr.shape[-len(destination_axes) : -1] != jitter_axes_shape:
+            raise ValueError("Got arrays with different sized jitter axes.")
+        if arr.shape[-1] - 2 * max_jitter <= 0:
+            raise ValueError("Jittered length is <= 0")
 
-    Parameters
-    ----------
-    tensor : torch.tensor
-        Tensor to be decoded.
-    num_seqs : int
-        Number of sequences to decode.
-        Default is 1.
+    rng = np.random.default_rng(seed)
+    starts = rng.integers(0, max_jitter + 1, jitter_axes_shape)
 
-    Returns
-    -------
-    seqs : np.ndarray
-        Numpy array of decoded sequences.
-    """
-    tokens = np.argmax(tensor.detach().numpy(), axis=1).reshape(num_seqs, -1)
-    seqs = np.array([decode_seq(_token2one_hot(token)) for token in tokens])
-    return seqs
+    sliced_arrs = []
+    for arr in arrays:
+        jittered_length = arr.shape[-1] - 2 * max_jitter
+        sliced = np.empty_like(arr)
+        gufunc_jitter_helper(arr, starts, max_jitter, sliced, axis=-1)  # type: ignore
+        sliced = sliced[..., :jittered_length]
+        sliced = np.moveaxis(sliced, destination_axes, [*jitter_axes, length_axis])
+        sliced_arrs.append(sliced)
 
-# EUGENe for generative models
-def generate_seqs_from_generator(generator, num_seqs : int = 1, normal : bool = False, device : str = "cpu"):
-    """
-    Generates random sequences from a generative generator.
+    return tuple(sliced_arrs)
+
+
+def random_seqs(
+    shape: Union[int, Tuple[int, ...]],
+    alphabet: NucleotideAlphabet,
+    seed: Optional[int] = None,
+):
+    """Generate random nucleotide sequences.
 
     Parameters
     ----------
-    generator : Basgeneratore
-        Generative generator used for sequence generation.
-    num_seqs : int
-        Number of sequences to decode.
-        Default is 1.
-    normal : bool
-        Whether to sample from a normal distribution instead of a uniform distribution.
-        Default is false.
+    shape : int, tuple[int]
+        Shape of sequences to generate
+    alphabet : NucleotideAlphabet
+        Alphabet to sample nucleotides from.
+    seed : int, optional
+        Random seed.
 
     Returns
     -------
-    seqs : np.ndarray
-        Numpy array of decoded sequences.
+    ndarray
+        Randomly generated sequences.
     """
-    if normal:
-        z = torch.Tensor(np.random.normal(0, 1, (num_seqs, generator.latent_dim)))
-    else: 
-        z = torch.rand(num_seqs, generator.latent_dim)
-    z = z.to(device)
-    fake = generator(z)
-    return seqs_from_tensor(fake.cpu(), num_seqs)
+    rng = np.random.default_rng(seed)
+    return rng.choice(alphabet.array, size=shape)
```

### Comparing `seqpro-0.0.1/seqpro/_helpers.py` & `seqpro-0.1.0/seqpro/deprecated/_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,59 @@
 import numpy as np
+
 np.random.seed(13)
 
 
 # VOCABS -- for DNA/RNA only for now
 DNA = ["A", "C", "G", "T"]
 RNA = ["A", "C", "G", "U"]
 COMPLEMENT_DNA = {"A": "T", "C": "G", "G": "C", "T": "A"}
 COMPLEMENT_RNA = {"A": "U", "C": "G", "G": "C", "U": "A"}
 
+
 # exact concise
 def _get_vocab(vocab):
     if vocab == "DNA":
         return DNA
     elif vocab == "RNA":
         return RNA
     else:
         raise ValueError("Invalid vocab, only DNA or RNA are currently supported")
 
+
 # exact concise
 def _get_vocab_dict(vocab):
     """
     Returns a dictionary mapping each token to its index in the vocabulary.
     Used in `_tokenize`.
     """
     return {l: i for i, l in enumerate(vocab)}
 
+
 # exact concise
 def _get_index_dict(vocab):
     """
     Returns a dictionary mapping each token to its index in the vocabulary.
     """
     return {i: l for i, l in enumerate(vocab)}
 
+
 # modified concise
 def _tokenize(seq, vocab="DNA", neutral_vocab=["N"]):
     """
     Convert sequence to integers based on a vocab
     Parameters
     ----------
-    seq: 
+    seq:
         sequence to encode
-    vocab: 
+    vocab:
         vocabulary to use
-    neutral_vocab: 
+    neutral_vocab:
         neutral vocabulary -> assign those values to -1
-    
+
     Returns
     -------
         List of length `len(seq)` with integers from `-1` to `len(vocab) - 1`
     """
     vocab = _get_vocab(vocab)
     if isinstance(neutral_vocab, str):
         neutral_vocab = [neutral_vocab]
@@ -64,24 +69,26 @@
 
     # current performance bottleneck
     return [
         vocab_dict[seq[(i * nchar) : ((i + 1) * nchar)]]
         for i in range(len(seq) // nchar)
     ]
 
+
 # my own
 def _sequencize(tvec, vocab="DNA", neutral_value=-1, neutral_char="N"):
     """
     Converts a token vector into a sequence of symbols of a vocab.
     """
-    vocab = _get_vocab(vocab) 
+    vocab = _get_vocab(vocab)
     index_dict = _get_index_dict(vocab)
     index_dict[neutral_value] = neutral_char
     return "".join([index_dict[i] for i in tvec])
 
+
 # modified concise
 def _token2one_hot(tvec, vocab="DNA", fill_value=None):
     """
     Converts an L-vector of integers in the range [0, D] into an L x D one-hot
     encoding. If fill_value is not None, then the one-hot encoding is filled
     with this value instead of 0.
     Parameters
@@ -99,38 +106,40 @@
     tvec_range = np.arange(len(tvec))
     tvec = np.asarray(tvec)
     arr[tvec[tvec >= 0], tvec_range[tvec >= 0]] = 1
     if fill_value is not None:
         arr[:, tvec_range[tvec < 0]] = fill_value
     return arr.astype(np.int8) if fill_value is None else arr.astype(np.float16)
 
+
 # modified dinuc_shuffle
 def _one_hot2token(one_hot, neutral_value=-1, consensus=False):
     """
     Converts a one-hot encoding into a vector of integers in the range [0, D]
     where D is the number of classes in the one-hot encoding.
     Parameters
     ----------
     one_hot : np.array
         L x D one-hot encoding
     neutral_value : int, optional
         Value to use for neutral values.
-    
+
     Returns
     -------
     np.array
         L-vector of integers in the range [0, D]
     """
     if consensus:
         return np.argmax(one_hot, axis=0)
     tokens = np.tile(neutral_value, one_hot.shape[1])  # Vector of all D
-    seq_inds, dim_inds = np.where(one_hot.transpose()==1)
+    seq_inds, dim_inds = np.where(one_hot.transpose() == 1)
     tokens[seq_inds] = dim_inds
     return tokens
 
+
 # pad and subset, exact concise
 def _pad(seq, max_seq_len, value="N", align="end"):
     seq_len = len(seq)
     assert max_seq_len >= seq_len
     if align == "end":
         n_left = max_seq_len - seq_len
         n_right = 0
@@ -145,14 +154,15 @@
 
     # normalize for the length
     n_left = n_left // len(value)
     n_right = n_right // len(value)
 
     return value * n_left + seq + value * n_right
 
+
 # exact concise
 def _trim(seq, maxlen, align="end"):
     seq_len = len(seq)
 
     assert maxlen <= seq_len
     if align == "end":
         return seq[-maxlen:]
@@ -162,21 +172,17 @@
         dl = seq_len - maxlen
         n_left = dl // 2 + dl % 2
         n_right = seq_len - dl // 2
         return seq[n_left:n_right]
     else:
         raise ValueError("align can be of: end, start or center")
 
+
 # modified concise
-def _pad_sequences(
-    seqs, 
-    maxlen=None, 
-    align="end", 
-    value="N"
-):
+def _pad_sequences(seqs, maxlen=None, align="end", value="N"):
     """
     Pads sequences to the same length.
     Parameters
     ----------
     seqs : list of str
         Sequences to pad
     maxlen : int, optional
@@ -202,40 +208,47 @@
     if maxlen is None:
         maxlen = max_seq_len
     else:
         maxlen = int(maxlen)
 
     if max_seq_len < maxlen:
         import warnings
+
         warnings.warn(
             f"Maximum sequence length ({max_seq_len}) is smaller than maxlen ({maxlen})."
         )
         max_seq_len = maxlen
 
     # check the case when len > 1
     for seq in seqs:
         if not len(seq) % len(value) == 0:
             raise ValueError("All sequences need to be dividable by len(value)")
     if not maxlen % len(value) == 0:
         raise ValueError("maxlen needs to be dividable by len(value)")
 
     padded_seqs = [
-        _trim(_pad(seq, max(max_seq_len, maxlen), value=value, align=align), maxlen, align=align)
-        for seq in seqs 
+        _trim(
+            _pad(seq, max(max_seq_len, maxlen), value=value, align=align),
+            maxlen,
+            align=align,
+        )
+        for seq in seqs
     ]
     return padded_seqs
 
+
 # my own
 def _is_overlapping(a, b):
     """Returns True if two intervals overlap"""
     if b[0] >= a[0] and b[0] <= a[1]:
         return True
     else:
         return False
 
+
 # my own
 def _merge_intervals(intervals):
     """Merges a list of overlapping intervals"""
     if len(intervals) == 0:
         return None
     merged_list = []
     merged_list.append(intervals[0])
@@ -245,71 +258,77 @@
             new_element = pop_element[0], max(pop_element[1], intervals[i][1])
             merged_list.append(new_element)
         else:
             merged_list.append(pop_element)
             merged_list.append(intervals[i])
     return merged_list
 
+
 # my own
 def _hamming_distance(string1, string2):
     """Find hamming distance between two strings. Returns inf if they are different lengths"""
     distance = 0
     L = len(string1)
     if L != len(string2):
         return np.inf
     for i in range(L):
         if string1[i] != string2[i]:
             distance += 1
     return distance
 
+
 # my own
 def _collapse_pos(positions):
     """Collapse neighbor positions of array to ranges"""
     ranges = []
     start = positions[0]
     for i in range(1, len(positions)):
         if positions[i - 1] == positions[i] - 1:
             continue
         else:
             ranges.append((start, positions[i - 1] + 2))
             start = positions[i]
     ranges.append((start, positions[-1] + 2))
     return ranges
 
+
 # exact dinuc_shuffle
 def _string_to_char_array(seq):
     """
     Converts an ASCII string to a NumPy array of byte-long ASCII codes.
     e.g. "ACGT" becomes [65, 67, 71, 84].
     """
     return np.frombuffer(bytearray(seq, "utf8"), dtype=np.int8)
 
+
 # exact dinuc_shuffle
 def _char_array_to_string(arr):
     """
     Converts a NumPy array of byte-long ASCII codes into an ASCII string.
     e.g. [65, 67, 71, 84] becomes "ACGT".
     """
     return arr.tostring().decode("ascii")
 
+
 # exact dinuc_shuffle
 def _one_hot_to_tokens(one_hot):
     """
     Converts an L x D one-hot encoding into an L-vector of integers in the range
     [0, D], where the token D is used when the one-hot encoding is all 0. This
     assumes that the one-hot encoding is well-formed, with at most one 1 in each
     column (and 0s elsewhere).
     """
     tokens = np.tile(one_hot.shape[1], one_hot.shape[0])  # Vector of all D
     seq_inds, dim_inds = np.where(one_hot)
     tokens[seq_inds] = dim_inds
     return tokens
 
+
 # exact dinuc_shuffle
 def _tokens_to_one_hot(tokens, one_hot_dim):
     """
     Converts an L-vector of integers in the range [0, D] to an L x D one-hot
     encoding. The value `D` must be provided as `one_hot_dim`. A token of D
     means the one-hot encoding is all 0s.
     """
     identity = np.identity(one_hot_dim + 1)[:, :-1]  # Last row is all 0s
-    return identity[tokens]
+    return identity[tokens]
```

### Comparing `seqpro-0.0.1/seqpro/_modifiers.py` & `seqpro-0.1.0/seqpro/deprecated/_modifiers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,61 @@
+import torch
 import numpy as np
-np.random.seed(13)
-from ._helpers import _string_to_char_array, _one_hot2token, _char_array_to_string, _token2one_hot
+from tqdm.auto import tqdm
+from _helpers import COMPLEMENT_DNA, COMPLEMENT_RNA
+from _helpers import _token2one_hot, _one_hot2token, _string_to_char_array, _one_hot2token, _char_array_to_string, _token2one_hot
+
+
+# my own
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
 
 # my own
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
+# my own
 def shuffle_seq(seq,  one_hot=False, seed=None):
     np.random.seed(seed)
     
     if one_hot:
         seq = np.argmax(seq, axis=-1)
         
     shuffled_idx = np.random.permutation(len(seq))
     shuffled_seq = np.array([seq[i] for i in shuffled_idx], dtype=seq.dtype)
     
     if one_hot:
         shuffled_seq = np.eye(4)[shuffled_seq]
-        
-    return shuffled_seq
+        return shuffled_seq
+    
+    else:
+        return np.array("".join(shuffled_seq))
 
 # my own
 def shuffle_seqs(seqs, one_hot=False, seed=None):
     return np.array([shuffle_seq(seq, one_hot=one_hot, seed=seed) for seq in seqs])
 
 # modified dinuc_shuffle
 def dinuc_shuffle_seq(
@@ -134,7 +170,8 @@
     if type(seqs) is str or type(seqs) is np.str_:
         seqs = [seqs]
 
     all_results = []
     for i in range(len(seqs)):
         all_results.append(dinuc_shuffle_seq(seqs[i], num_shufs=num_shufs, rng=rng))
     return np.array(all_results)
+
```

