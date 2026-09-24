# mooninfer

Run a model.

> **Status: planned.** The repository is set up; nothing is
> implemented yet.

The four libraries under it each answer one question — what the file says, what
a tensor is, what the device can do, what a token is. This one answers the
remaining ones: which weights go where, what to keep between steps, and which
token comes next.

| Package | What it covers |
|:--|:--|
| `model` | The architecture: which tensors, in which order |
| `cache` | The keys and values kept between steps, and when to drop them |
| `sample` | Choosing the next token: temperature, top-k, top-p, repetition |
| `serve` | An HTTP surface over [`moonapi`](https://github.com/moonbitstack/moonapi) |

Built on [`moongguf`](https://github.com/moonbitstack/moongguf),
[`moonggml`](https://github.com/moonbitstack/moonggml),
[`moonwgpu`](https://github.com/moonbitstack/moonwgpu) and
[`moontoken`](https://github.com/moonbitstack/moontoken) — four libraries that
are each worth having on their own, which is why they are not packages in here.

## Install

```bash
moon add moonbitstack/mooninfer
```

## Licence

Apache-2.0. See [LICENSE](LICENSE).
