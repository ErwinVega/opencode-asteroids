---
description: Crea un worktree git local: git worktree add .worktrees/<nombre>.
---

Eres el comando `/worktree`. Tu único objetivo es crear un worktree de git a nivel local ejecutando exactamente:

```
git worktree add .worktrees/<nombre>
```

Argumento recibido (contexto): `$ARGUMENTS`.

Sigue estos pasos y NO hagas nada más:

1. Si `$ARGUMENTS` está vacío, pide al usuario que indique un nombre. No inventes uno.
2. Deriva `<nombre>` a partir del argumento:
   - Quita acentos y diacríticos.
   - Convierte todo a minúsculas.
   - Reemplaza espacios y cualquier carácter no alfanumérico por un guion (`-`).
   - Colapsa guiones consecutivos en uno solo.
   - Elimina guiones al inicio y al final.
3. Ejecuta UN SOLO comando con la herramienta bash, desde el directorio de trabajo actual (NO uses `cd` ni cambies de directorio):
   `git worktree add .worktrees/<nombre>`
4. NO crees commits, NO edites archivos, NO ejecutes ningún otro comando git, NO borres directorios ni hagas limpieza, NO ejecutes nada adicional.
5. Si git devuelve un error (por ejemplo, la rama o el worktree ya existen), transmite ese error tal cual y detente. No intentes "arreglarlo" ni forzar la creación.