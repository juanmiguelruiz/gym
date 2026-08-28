# gym

Base de una webapp con Next.js, TypeScript, Tailwind CSS y pnpm.

## Requisitos

- Node.js 26.8.1 (última release estable), usando `.nvmrc`.
- pnpm 11.4.0.

Con `nvm`:

```bash
nvm install
nvm use
corepack enable
corepack prepare pnpm@11.4.0 --activate
```

## Desarrollo

```bash
pnpm install
pnpm dev
```

La aplicación queda disponible en <http://localhost:3000>.

Para trabajar desde otra máquina o mediante el navegador remoto de Codex:

```bash
pnpm dev:remote
```

Este script escucha en `0.0.0.0` y usa el puerto indicado por `PORT` (3000 por defecto). El acceso remoto debe hacerse mediante el mecanismo de forwarding/túnel de la máquina o entorno de desarrollo; no se publica directamente en Internet.

Ejemplo de forwarding SSH desde tu equipo:

```bash
ssh -L 3000:localhost:3000 usuario@servidor
```

Después abre <http://localhost:3000> en tu navegador. Los cambios guardados en el repositorio se reflejan automáticamente gracias a Fast Refresh.

## Comandos útiles

```bash
pnpm lint       # Comprueba el código
pnpm build      # Genera la build de producción
pnpm start:remote
```
