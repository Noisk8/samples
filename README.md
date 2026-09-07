# samples
banco de samples para livecoding

## WebFoxDot loops

Los audios se cargan y se usan exclusivamente como loops mediante `loadloop`.

```python
base = "https://raw.githubusercontent.com/Noisk8/samples/main/samples-prueba/"
loadloop("una", base + "una.wav")
loadloop("voz1", base + "voz1.wav")
loadloop("voz2", base + "voz2.wav")
loadloop("voz3", base + "voz3.wav")
loadloop("vrisas", base + "vrisas.wav")
loadloop("lenin", base + "lenin.wav")
loadloop("lenin_camino_al_socialismo", base + "lenin_camino_al_socialismo.wav")
```

Después de registrar un audio, se llama por su nombre:

```python
p1 >> loop("lenin", dur=4)
p2 >> loop("lenin_camino_al_socialismo", dur=4)
```
