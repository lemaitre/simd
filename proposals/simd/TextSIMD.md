# Text format for SIMD

### v128.const

The `v128.const` instruction has multiple valid text formats corresponding to
different lane interpretations. The valid text formats are

```
v128.const i8x16 i8 i8 i8 i8 i8 i8 i8 i8 i8 i8 i8 i8 i8 i8 i8 i8
v128.const i16x8 i16 i16 i16 i16 i16 i16 i16 i16
v128.const i32x4 i32 i32 i32 i32
v128.const i64x2 i64 i64
v128.const f32x4 f32 f32 f32 f32
v128.const f64x2 f64 f64
```

The canonical text format used for printing `v128.const` instructions is

```
v128.const i32x4 0xNNNNNNNN 0xNNNNNNNN 0xNNNNNNNN 0xNNNNNNNN
```

### Shuffling using immediate indices

```
v8x16.shuffle2_imm i5 i5 i5 i5 i5 i5 i5 i5 i5 i5 i5 i5 i5 i5 i5 i5
v16x8.shuffle2_imm i4 i4 i4 i4 i4 i4 i4 i4
v32x4.shuffle2_imm i3 i3 i3 i3
v64x2.shuffle2_imm i2 i2
```