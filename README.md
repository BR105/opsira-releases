# opsira-releases

Archivos públicos que descarga la app (el código vive en un repo privado aparte).

## Modelos de IA (release `modelos-v1`)

Se descargan solo la primera vez que se usa cada herramienta y corren **en el teléfono**: ninguna foto se sube a un servidor.

| Archivo | Uso | Origen | Licencia |
|---|---|---|---|
| `migan_pipeline_v2.onnx` (26.8 MB) | Eliminar avanzado (inpainting) | [MI-GAN](https://github.com/Picsart-AI-Research/MI-GAN), Picsart AI Research | MIT |
| `ggml-base-q5_1.bin` (56.9 MB) | Subtítulos automáticos de video (voz a texto) | [Whisper](https://github.com/openai/whisper) base, OpenAI; formato ggml cuantizado de [whisper.cpp](https://github.com/ggml-org/whisper.cpp) (Georgi Gerganov) | MIT |
| `realesr-general-x4v3.onnx` (4.6 MB) | Mejorar HD (super-resolución ×4) | [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN), Xintao Wang; exportación ONNX de [tinier-upscale-models](https://huggingface.co/jonathanst29/tinier-upscale-models) | BSD-3-Clause |

SHA-256:
- `migan_pipeline_v2.onnx`: `6F1F3530A1A2324B19752018CE756088B07973CDA8D7D890034ACE5C8A48C40B`
- `realesr-general-x4v3.onnx`: `924EBAD6532777303582D4CE7811849B88869231A3AE7093E0F21200249DF8D5`
- `ggml-base-q5_1.bin`: `422F1AE452ADE6F30A004D7E5C6A43195E4433BC370BF23FAC9CC591F01A8898`

Los textos completos de las licencias están en [`LICENCIAS-MODELOS.md`](LICENCIAS-MODELOS.md).
