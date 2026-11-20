# Personal fork engine pin

`maestro-0.1.2-9de7437.tgz` is the `npm pack` distribution from [Maestro commit `9de7437`](https://github.com/ychengbao/maestro/commit/9de74377bc2f9ed60ff3a1bfce46a751a79c8b79), based on `v0.1.2`. It retires an orphaned `.exit` before dispatching a resumed Pi child. The Git installation of `personal-ui` uses this archive directly; no postinstall patch is required.

To rebuild, check out the linked commit in the engine repository and run `npm ci && npm pack` with Node 26.12.1. When an official release includes the fix, switch the dependency and pin checks back to that exact registry version and remove this archive.
