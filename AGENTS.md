<!-- g360:agents:begin -->
# AGENTS.md — g360-Horas_Extras

Generador de planillas de horas extras en formato Excel corporativo. Forma parte de la familia de microherramientas G360 para gestión de tiempos y planificación

> El bloque entre los markers `g360:agents` lo genera `g360 agents` y se
> regenera sin perder lo que escribas afuera.

## Verificación

Un solo comando deja el repo listo y verifica que todo esté en verde:

```bash
pip install -r requirements.lock
python -m compileall src
```

- Stack: python (pip)
- Tests: sin tests (compileall)
- ⚠️ Sin suite de tests: agregá tests de comportamiento con `pytest`; compileall solo detecta errores de sintaxis.

## Instalación

```bash
pip install -r requirements.lock
```


## Estructura

- `src/`
- `src/main.py`
- `run.py`
- `build.py`

## Convenciones

- Tests con `pytest` en `tests/`.
- Dependencias declaradas en `requirements.txt`.
- Comentarios que expliquen el *por qué*, no el *qué*.

## Reglas de este repo

- **Autosuficiente**: `git clone` + el comando de verificación debe dejar la app levantada y los tests en verde, sin red y sin ayuda de una persona.
- **Tests honestos**: nada de `it.skip`, `pytest.mark.skip`, `xfail` ni `assert true` para forzar verde.
- **Entorno declarativo**: toda variable de entorno va en `.env.example` con un default seguro.
- **Sin paths de tu máquina**: nada de rutas absolutas locales ni secretos en el código.
- **Evidencia**: al entregar, reportá el comando que corriste y su salida. Si no pudiste verificar, decilo.
<!-- g360:agents:end -->
