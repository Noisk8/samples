# samples
banco de samples para livecoding

## WebFoxDot

Este repositorio se puede cargar como un pack remoto:

```python
loadpack("https://raw.githubusercontent.com/Noisk8/samples/main/pack.json")
```

Los samples se organizan así:

- `d`: `dos.wav`
- `f`: `french.wav`
- `p`: `una.wav`
- `v`: `voz1.wav`, `voz2.wav`, `voz3.wav`
- `r`: `vrisas.wav`

Por ejemplo, `play("v", sample=1)` usa `voz2.wav`.

## Loops

`loop` necesita registrar cada audio con `loadloop` antes de usarlo:

```python
base = "https://raw.githubusercontent.com/Noisk8/samples/main/samples-prueba/"
loadloop("dos", base + "dos.wav")
loadloop("french", base + "french.wav")
loadloop("una", base + "una.wav")
loadloop("voz1", base + "voz1.wav")
loadloop("voz2", base + "voz2.wav")
loadloop("voz3", base + "voz3.wav")
loadloop("vrisas, base + "vrisas.wav")
```

Después de cargarlo, se llama por nombre:

```python
p1 >> loop("voz1", dur=4)
```
