> Instale isso no CMD antes.
`pip install pyautogui`

---

**Copia e cola:**

```
import pyautogui
import time

print("--- MIRA DO SNIPER ---")
print("Mova o mouse para a posição desejada.")
print("As coordenadas serão atualizadas a cada segundo.")
print("Pressione CTRL+C para sair.")

try:
    while True:
        x, y = pyautogui.position()
        positionStr = 'X: ' + str(x).rjust(4) + ' Y: ' + str(y).rjust(4)
        print(positionStr, end='')
        print('\b' * len(positionStr), end='', flush=True)
        time.sleep(1)
except KeyboardInterrupt:
    print('\n--- Mira travada. ---')
```
