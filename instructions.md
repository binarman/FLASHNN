kernel of interest: _paged_attn_w_mma_kernel

config of interest for mfma 16x16 case: num_warps=2, num_stages=1

profiling command:

```
rocprofv2 -i att.txt --plugin att auto --mode file -d output python3 benchmark/benchmark_paged_attn.py
```
