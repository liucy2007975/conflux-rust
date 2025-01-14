# 1.1.1

## Improvements

- Reduce delay in logs pub-sub; now we send logs immediately after they become available.
- Implement Execution Trace functionality. It includes detailed call/create/return/internal_transfer events being triggered by a transfer. Inspecting the trace information will enable the applications like conflux-scan to be able to track all transfers of CFX accurately. 

# 1.1.0

## Incompatible changes

- CIP-38: Reduce the block base reward to 2 CFX from the epoch number 3,615,000.
- CIP-39: Blocks from the height 3,615,000 (included) are required to set the first element of their `custom` field in the header to `[1]`.

## Improvements
- Return the `custom` field in the block header for related RPCs (`cfx_getBlockByHash`, `cfx_getBlockByHashWithPivotAssumption`, `cfx_getBlockByEpochNumber`).
